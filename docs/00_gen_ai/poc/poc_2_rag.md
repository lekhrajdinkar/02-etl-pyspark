## Infra : s3, dynamo, IAM role
- [terraform workspace : genai-poc-2-rag](https://app.terraform.io/app/lekhrajdinkar-org/workspaces/genai-poc-2-rag)
- **terraform apply**
- [run HCP](https://app.terraform.io/app/lekhrajdinkar-org/genai-poc-2-rag/runs/run-TyiNbuDn4Veg3hrj)
    - [bedrock_rag_execution_role](https://us-east-1.console.aws.amazon.com/iam/home?region=us-east-1#/roles/details/bedrock_rag_execution_role?section=permissions) 
    - [genai-rag-demo-lekhrajdinkar-bucket](https://us-east-1.console.aws.amazon.com/s3/buckets/genai-rag-demo-lekhrajdinkar-bucket?region=us-east-1&bucketType=general)
    - [DynamoDB table - rag_chunks](https://us-east-1.console.aws.amazon.com/dynamodbv2/home?region=us-east-1#table?name=rag_chunks)

## project structure
```
src/AIModule/poc_2_rag/
├── embedder.py           # Call Bedrock embedding model
├── rag_ingest.py         # Load files, chunk, embed, and store to DynamoDB/S3
├── dynamo_client.py      # DynamoDB helper for saving & querying
├── s3_client.py          # S3 file upload
├── utils.py              # Chunking, cleaning
└── sample_docs/          # Put PDFs or .md here
```

## Steps
```
✅ Step 1: Setup RAG Ingestion Pipeline

1. 📄 rag_ingest.py 
Document Ingestion Script
Loads .md or .txt files
Chunks content
Embeds using Bedrock (co.embed.multilingual-v1)

Stores:
  S3 :: Original file
  DynamoDB :: Chunk metadata
```

---
## Screenshot

![img.png](img.png)

