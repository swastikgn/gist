---
author: Swastik G N
pubDatetime: 2025-03-18T07:27:47Z
modDatetime: 2025-03-18T07:27:54Z
title: Running postgresql container without password.
slug: postgresql-container-without-password
featured: false
draft: false
tags:
  - postgresql
  - docker 
  - container
description:
  command to run postgres without password and DATABASE_URL to connect to the database.
---

## Command to run postgresql container
```bash 
 docker run -d --name my-postgres -e POSTGRES_HOST_AUTH_METHOD=trust -p 5432:5432 postgres
```

## DATABASE_URL to connect to database 
```
DATABASE_URL="postgresql://postgres@localhost:5432/postgres"
```