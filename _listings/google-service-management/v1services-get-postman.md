{
  "info": {
    "name": "Google Service Management API Get Services",
    "_postman_id": "10eee3b6-aba5-4190-bcec-02c7288fa58f",
    "description": "Lists managed services.\n\nReturns all public services. For authenticated users, also returns all\nservices the calling user has \"servicemanagement.services.get\" permission\nfor.\n\n**BETA:** If the caller specifies the `consumer_id`, it returns only the\nservices enabled on the consumer. The `consumer_id` must have the format\nof \"project:{PROJECT-ID}\".",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Service",
      "item": [
        {
          "id": "d5eed9c1-4530-4fd7-8a65-cd8e35fe78e1",
          "name": "servicemanagement.services.list",
          "request": {
            "url": "http://servicemanagement.googleapis.com/v1/services?consumerId=%7B%7D&pageSize=%7B%7D&pageToken=%7B%7D&producerProjectId=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Lists managed services.\n\nReturns all public services. For authenticated users, also returns all\nservices the calling user has \"servicemanagement.services.get\" permission\nfor.\n\n**BETA:** If the caller specifies the `consumer_id`, it returns only the\nservices enabled on the consumer. The `consumer_id` must have the format\nof \"project:{PROJECT-ID}\"."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "860ecd9d-bfd8-4dc0-9fba-d51082e39a2a"
            }
          ]
        }
      ]
    }
  ]
}