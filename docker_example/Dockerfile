FROM python:3.11-slim

ENV LANGFLOW_HOME=/home/langflow
WORKDIR ${LANGFLOW_HOME}

RUN pip install langflow

# Expor a porta correta explicitamente
EXPOSE 7860

# Comando corrigido e atualizado
CMD ["sh", "-c", "langflow run --host 0.0.0.0 --port ${PORT:-7860}"]
