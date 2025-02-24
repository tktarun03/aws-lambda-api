# aws-lambda-api

A simple AWS Lambda function integrated with API Gateway for a serverless API.

## 🚀 Features
- Uses **AWS Lambda** for serverless computing.
- Integrated with **API Gateway** to expose as an API endpoint.
- Fully scalable and cost-efficient.

## 📂 Project Structure
```
aws-lambda-api/
│── src/
│   ├── lambda_function.py  # AWS Lambda function
│── README.md
```

## 🛠 Deployment & Usage

1. Zip and upload `lambda_function.py` to AWS Lambda:
   ```bash
   zip function.zip src/lambda_function.py
   ```

2. Deploy via AWS Console or AWS CLI:
   ```bash
   aws lambda create-function --function-name myLambdaAPI    --runtime python3.8 --role <IAM_ROLE> --handler lambda_function.lambda_handler    --zip-file fileb://function.zip
   ```

3. Attach **API Gateway** to expose Lambda as a REST API.

4. Invoke function manually:
   ```bash
   aws lambda invoke --function-name myLambdaAPI response.json
   ```

## 👨‍💻 About the Author

🚀 Created by [Arunkumar Thamilarasu](https://github.com/tktarun03) | UI Technical Architect | AWS & Serverless Expert

## ⭐ Contribute & Support
- Fork & Star this repository! ⭐
- Submit Issues and PRs to improve the Lambda function.

---
🎯 **Follow me on GitHub**: [@tktarun03](https://github.com/tktarun03)
