---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d27606707edb8c662a1db2ab3599d6574956482b0be4b38f699f779273da940d
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56904225"
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