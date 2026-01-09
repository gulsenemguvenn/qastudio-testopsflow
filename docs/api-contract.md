# API Contract (Draft) – QAStudio TestOpsFlow

## Auth
- POST /api/auth/register
- POST /api/auth/login
- GET  /api/users/me

## Workspaces
- POST /api/workspaces
- GET  /api/workspaces
- GET  /api/workspaces/{workspaceId}
- POST /api/workspaces/{workspaceId}/members
- GET  /api/workspaces/{workspaceId}/members
- DELETE /api/workspaces/{workspaceId}/members/{userId}

## Projects
- POST /api/workspaces/{workspaceId}/projects
- GET  /api/workspaces/{workspaceId}/projects
- GET  /api/projects/{projectId}
- POST /api/projects/{projectId}/members
- GET  /api/projects/{projectId}/members

## Issues
- POST /api/projects/{projectId}/issues
- GET  /api/projects/{projectId}/issues?type=&status=&assigneeId=&q=&page=&size=
- GET  /api/issues/{issueId}
- PUT  /api/issues/{issueId}
- PATCH /api/issues/{issueId}/status
- DELETE /api/issues/{issueId}

## Sprints
- POST /api/projects/{projectId}/sprints
- GET  /api/projects/{projectId}/sprints
- POST /api/sprints/{sprintId}/start
- POST /api/sprints/{sprintId}/complete
- GET  /api/sprints/{sprintId}/report

## Comments
- POST /api/issues/{issueId}/comments
- GET  /api/issues/{issueId}/comments
