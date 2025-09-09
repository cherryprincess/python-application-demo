# Python Flask Application Demo

A simple Flask application that calculates change for given dollar amounts.

## Features
- Change calculation API
- Health check endpoints
- Logging and monitoring
- Docker containerization
- Kubernetes deployment ready
- CI/CD pipeline with GitHub Actions

## API Endpoints
- `GET /` - Welcome message and health info
- `GET /health` - Health check
- `GET /change/<dollar>/<cents>` - Calculate change

## Local Development
```bash
pip install -r requirements.txt
python app.py
```

## Docker
```bash
docker build -t python-flask-app .
docker run -p 8080:8080 python-flask-app
```

## Kubernetes Deployment
```bash
kubectl apply -f k8s/
```

## Security Features
- Non-root container execution
- Security contexts and policies
- Resource limits
- Network policies
- Vulnerability scanning with Trivy
