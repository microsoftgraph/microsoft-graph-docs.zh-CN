---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 82104926dd05e1a5e3c7e1602f15199d1272c6e2
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48981087"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

UnifiedRoleDefinition unifiedRoleDefinition = new UnifiedRoleDefinition();
unifiedRoleDefinition.description = "Update basic properties of application registrations";
unifiedRoleDefinition.displayName = "Application Registration Support Administrator";
LinkedList<UnifiedRolePermission> rolePermissionsList = new LinkedList<UnifiedRolePermission>();
UnifiedRolePermission rolePermissions = new UnifiedRolePermission();
LinkedList<String> allowedResourceActionsList = new LinkedList<String>();
allowedResourceActionsList.add("microsoft.directory/applications/basic/read");
rolePermissions.allowedResourceActions = allowedResourceActionsList;
rolePermissionsList.add(rolePermissions);
unifiedRoleDefinition.rolePermissions = rolePermissionsList;
unifiedRoleDefinition.isEnabled = false;

graphClient.roleManagement().directory().roleDefinitions()
    .buildRequest()
    .post(unifiedRoleDefinition);

```