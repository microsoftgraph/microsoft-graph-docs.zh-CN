---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: cdc869adbb34be07937862bc19609f03b0a47833e6aca8f220dc66036e6948ab
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57161838"
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