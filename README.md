# Back-End-Development-Pictures

IBM Back-End Development Capstone: Flask REST API for concert pictures.

## Environment Setup
- Repository created from the provided IBM template.
- Cloud IDE environment initialized using `bin/setup.sh`.
- Python 3.9; virtual environment named `venv` at `~/venv`, created by the supplied setup script with `python3.9 -m venv ~/venv`.
- Activate it with `source ~/venv/bin/activate`.
- The setup script's Python environment and dependency installation steps completed successfully in IBM Skills Network Cloud IDE, and all supplied API tests subsequently passed.

## API
- `GET /health`: service health.
- `GET /count`: number of pictures.
- `GET /picture`: all pictures.
- `GET /picture/<id>`: one picture, or 404.
- `POST /picture`: create a picture, or 302 for a duplicate identifier.
- `PUT /picture/<id>`: update an existing picture.
- `DELETE /picture/<id>`: delete an existing picture.

Picture data is held in memory, initialized from `backend/data/pictures.json`.

## Verification
Run `python -m pytest -v tests/test_api.py`. All 11 supplied tests passed in IBM Skills Network Cloud IDE.
