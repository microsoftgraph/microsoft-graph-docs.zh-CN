---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 81638c813347d9faf7123935dc3c79c73bd8840e
ms.sourcegitcommit: 503c72036c376a30e08c29df8e7730a7afcab66e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/10/2021
ms.locfileid: "52868962"
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