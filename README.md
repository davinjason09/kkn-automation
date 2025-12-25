# KKN Attendance Automation

A simple program that can automatically (soon™) submits your KKN-PPM UGM attendance using the new VNEXT Checkpoint API

---

## Getting Started

There are currently only one way to run this, for planned feature see [TODO](#todo)

1. Clone the repository

```sh
git clone 'repo_url'
cd 'repo_loc'
```

2. Setup the Python environment

- If you're using `pip`:
  - Set up a Virtual environment

    ```sh
    python -m venv .venv
    source .venv/bin/activate
    ```

  - Install the dependencies

    ```sh
    pip install -r requirements.txt
    ```

- If you're using [`uv`](https://github.com/astral-sh/uv/)

  ```sh
  uv sync
  ```

3. Create the Environment File

Create a file named `.env` in the project's root directory.

4. Configure your settings

Copy the template below into your `.env` or see [example](./.env.example).

```sh
# --- QR Code Location Value (Required) ---
QR_CODE_VALUE=the_qr_value

# --- KKN Location Settings (Required) ---
KKN_LOCATION_LATITUDE=-7.9547226
KKN_LOCATION_LONGITUDE=110.2788225
KKN_LOCATION_RADIUS_METERS=50
```

5. Run `main.py`

## TODO

- Automation (Docker/Termux/GitHub actions?)
- More features related to KKN (logbook, etc.)

---
