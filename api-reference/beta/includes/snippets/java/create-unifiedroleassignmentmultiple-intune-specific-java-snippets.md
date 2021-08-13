---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: bc5f21931fffa7feb46a301e0c3141518804626ce3343b0c07b1523576e53ea1
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54274570"
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
LinkedList<String> appScopeIdsList = new LinkedList<String>();
appScopeIdsList.add("allDevices");
unifiedRoleAssignmentMultiple.appScopeIds = appScopeIdsList;

graphClient.roleManagement().deviceManagement().roleAssignments()
    .buildRequest()
    .post(unifiedRoleAssignmentMultiple);

```