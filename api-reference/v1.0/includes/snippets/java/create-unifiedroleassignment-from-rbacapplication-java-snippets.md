---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d53afb714bca4d467c35fd883463d83b35ba3440
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59061035"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

UnifiedRoleAssignment unifiedRoleAssignment = new UnifiedRoleAssignment();
unifiedRoleAssignment.roleDefinitionId = "c2cf284d-6c41-4e6b-afac-4b80928c9034";
unifiedRoleAssignment.principalId = "f8ca5a85-489a-49a0-b555-0a6d81e56f0d";
unifiedRoleAssignment.directoryScopeId = "/";

graphClient.roleManagement().directory().roleAssignments()
    .buildRequest()
    .post(unifiedRoleAssignment);

```