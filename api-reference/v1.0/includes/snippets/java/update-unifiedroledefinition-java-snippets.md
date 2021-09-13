---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 38e9551187d03ee0cbd38d1728315eb321885a0f
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59097843"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

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

graphClient.roleManagement().directory().roleDefinitions("0d55728d-3e24-4309-9b1b-5ac09921475a")
    .buildRequest()
    .patch(unifiedRoleDefinition);

```