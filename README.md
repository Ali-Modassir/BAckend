# GroupService API Documentation

This document provides information about the GroupService API endpoints and their usage.

## Table of Contents

- [Introduction](#introduction)
- [Endpoints](#endpoints)
  - [Add Group](#add-group)
  - [Update Group](#update-group)
  - [Get Project](#get-project)
  - [Get Agent List](#get-agent-list)
  - [Delete Group](#delete-group)

## Introduction

The GroupService API allows you to manage groups and related information within the system. You'll need a valid session token and project ID to make requests to these endpoints.

## Endpoints

### Add Group

Create a new group.

- **Method:** POST
- **URL:** `https://h-dev-apigateway.byjus.onl/wfms-configuration-management/wfms/groupManagement/v1/groups`
- **Headers:**
  - `sessionToken`: Your session token
  - `projectId`: Project ID (e.g., 3)
- **Request Body:**
  ```json
  {
    "groupName": "groupName25",
    "description": "string",
    "ownerEmail": "string",
    "groupEmail": "string",
    "createdAt": "2023-04-26T08:19:29.156Z",
    "projectId": 3,
    "agent": [
      {
        "firstName": "string",
        "lastName": "string",
        "email": "string"
      }
    ]
  }
Response: No response details provided.
Update Group
Update an existing group.

Method: PUT
URL: https://h-dev-apigateway.byjus.onl/wfms-configuration-management/wfms/groupManagement/v1/groups/25
Headers: Same as above
Request Body:
json
Copy code
{
  "groupName": "group25",
  "description": "string",
  "ownerEmail": "string",
  "groupEmail": "string",
  "createdAt": "2023-04-27T09:51:43.573Z",
  "projectId": 3,
  "agent": [
    {
      "firstName": "string",
      "lastName": "string",
      "email": "string"
    }
  ]
}
Response: No response details provided.
Get Project
Get project information.

Method: GET
URL: http://localhost:8080/wfms-configuration-management/wfms/groupManagement/v1/groups
Headers: Same as above
Query Parameters:
projectId: Project ID (e.g., 3)
Response: No response details provided.
Get Agent List
Get a list of agents.

Method: GET
URL: https://h-dev-apigateway.byjus.onl/wfms-configuration-management/wfms/groupManagement/v1/agentList
Headers: Same as above
Query Parameters:
projectId: Project ID (e.g., 3)
pageSize: Number of items per page (e.g., 20)
pageNumber: Page number (e.g., 0)
Response: No response details provided.
Delete Group
Delete a group.

Method: DELETE
URL: http://localhost:8080/wfms-configuration-management/wfms/groupManagement/v1/groups/11
Headers: Same as above
Response: No response details provided.




