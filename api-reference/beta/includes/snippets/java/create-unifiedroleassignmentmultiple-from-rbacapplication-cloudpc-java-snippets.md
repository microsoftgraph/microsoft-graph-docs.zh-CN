---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5e6050fe15a398acf38a7a5b7ed9d2f2404a0dbf8f66b7a4df1de978bd25869e
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57328744"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

UnifiedRoleAssignmentMultiple unifiedRoleAssignmentMultiple = new UnifiedRoleAssignmentMultiple();
unifiedRoleAssignmentMultiple.displayName = "My test role assignment 1";
unifiedRoleAssignmentMultiple.description = "My role assignment description";
unifiedRoleAssignmentMultiple.roleDefinitionId = "b5c08161-a7af-481c-ace2-a20a69a48fb1";
LinkedList<String> principalIdsList = new LinkedList<String>();
principalIdsList.add("f8ca5a85-489a-49a0-b555-0a6d81e56f0d");
principalIdsList.add("c1518aa9-4da5-4c84-a902-a31404023890");
unifiedRoleAssignmentMultiple.principalIds = principalIdsList;

graphClient.roleManagement().cloudPC().roleAssignments()
    .buildRequest()
    .post(unifiedRoleAssignmentMultiple);

```