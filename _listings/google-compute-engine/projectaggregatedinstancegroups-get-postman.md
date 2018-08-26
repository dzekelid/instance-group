{
  "info": {
    "name": "Compute Engine",
    "_postman_id": "fefd12cf-90d6-4af5-948c-b9cc6cde8b98",
    "description": "Creates and runs virtual machines on Google Cloud Platform.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "instance group",
      "item": [
        {
          "id": "4096a035-3e86-4824-8e94-ac4c4c81021b",
          "name": "compute.instanceGroups.aggregatedList",
          "request": {
            "url": {
              "protocol": "http",
              "host": "www.googleapis.com",
              "path": [
                "compute",
                "v1",
                "projects",
                ":project/aggregated/instanceGroups"
              ],
              "query": [
                {
                  "key": "filter",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "maxResults",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "orderBy",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "pageToken",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "project",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieves the list of instance groups and sorts them by zone"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "8f7c5e0f-76ed-4976-8d3b-4c3902a800b1"
            }
          ]
        }
      ]
    }
  ]
}