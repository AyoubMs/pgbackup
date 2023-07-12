# pgbackup

==========

CLI for backing up remote PostgreSQL databases locally or to AWS S3.

## Usage

Pass in a full database URL, the storage driver, and destination.

S3 Example w/ bucket name:

```bash
$ pgbackup postgres://bob@example.com:5432/db_one --driver s3 backups
```

Local Example w/ local path:

```bash
$ pgbackup postgres://bob@example.com:5432/db_one --driver local /
var/local/db_one/backups
```

## Installation From Source

To install the package after you've cloned the repository, you'll
want to run the following command from within the project directory:

```bash
$ pip install --user -e .
```

## Preparing for Development

Follow these steps to start developing with this project:

1. Ensure `python` is installed
2. Clone repository: `git clone git@github.com:AyoubMs/pgbackup`
3. `cd` into the repository
4. Create virtualenv: `python -m venv pgbackup`
5. Activate virtualenv: `.\pgbackup\Scripts\Activate.ps1`
