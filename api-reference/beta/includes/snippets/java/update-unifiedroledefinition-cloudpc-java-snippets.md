---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 22f8a31ce1a0de6787d403e5575491e50163dc5a
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62089122"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

UnifiedRoleDefinition unifiedRoleDefinition = new UnifiedRoleDefinition();
unifiedRoleDefinition.description = "Update basic properties and permission of application registrations";
unifiedRoleDefinition.displayName = "ExampleCustomRole";
LinkedList<UnifiedRolePermission> rolePermissionsList = new LinkedList<UnifiedRolePermission>();
UnifiedRolePermission rolePermissions = new UnifiedRolePermission();
LinkedList<String> allowedResourceActionsList = new LinkedList<String>();
allowedResourceActionsList.add("Microsoft.CloudPC/CloudPCs/Read");
allowedResourceActionsList.add("Microsoft.CloudPC/CloudPCs/Reprovision");
rolePermissions.allowedResourceActions = allowedResourceActionsList;
rolePermissionsList.add(rolePermissions);
unifiedRoleDefinition.rolePermissions = rolePermissionsList;

graphClient.roleManagement().cloudPC().roleDefinitions("b7f5ddc1-b7dc-4d37-abce-b9d6fc15ffff")
    .buildRequest()
    .patch(unifiedRoleDefinition);

```