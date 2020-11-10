---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 20c73cf8ea9cfff467ebb29b7703e5a87b1cc96c
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48978103"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

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