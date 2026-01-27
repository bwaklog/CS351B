FROM python:3.10-slim

WORKDIR /app
RUN pip install --no-cache-dir flask scikit-learn joblib

COPY app.py .
COPY spam_classifier_model.pkl .
COPY tfidf_vectorizer.pkl .
COPY ./templates /app/templates/

EXPOSE 5000

CMD ["python", "app.py"]
