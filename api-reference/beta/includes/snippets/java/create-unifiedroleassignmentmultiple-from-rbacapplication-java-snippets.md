---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 90047c2cba386a24ea3d50b5de8cc69904a002f6
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50983419"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

UnifiedRoleAssignmentMultiple unifiedRoleAssignmentMultiple = new UnifiedRoleAssignmentMultiple();
unifiedRoleAssignmentMultiple.displayName = "My test role assignment 1";
unifiedRoleAssignmentMultiple.roleDefinitionId = "c2cf284d-6c41-4e6b-afac-4b80928c9034";
LinkedList<String> principalIdsList = new LinkedList<String>();
principalIdsList.add("f8ca5a85-489a-49a0-b555-0a6d81e56f0d");
principalIdsList.add("c1518aa9-4da5-4c84-a902-a31404023890");
unifiedRoleAssignmentMultiple.principalIds = principalIdsList;
LinkedList<String> directoryScopeIdsList = new LinkedList<String>();
directoryScopeIdsList.add("28ca5a85-489a-49a0-b555-0a6d81e56f0d");
directoryScopeIdsList.add("8152656a-cf9a-4928-a457-1512d4cae295");
unifiedRoleAssignmentMultiple.directoryScopeIds = directoryScopeIdsList;

graphClient.roleManagement().deviceManagement().roleAssignments()
    .buildRequest()
    .post(unifiedRoleAssignmentMultiple);

```