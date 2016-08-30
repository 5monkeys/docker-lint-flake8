# flake8 (Python 3 / Alpine)


Minimal flake8 image using Alpine.


# Usage

## Example usage via Docker Compose

### docker-compose.yml

```yaml
version: "2"
services:
  lint-py:
    image: 5monkeys/lint-flake8
    volumes:
      - "./setup.cfg:/setup.cfg"
      - ".:/code"
```

### Running

```bash
$  docker-compose run --rm lint-py
```
