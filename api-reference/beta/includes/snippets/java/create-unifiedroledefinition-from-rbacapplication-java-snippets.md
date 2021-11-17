---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0dc32ba3a7bfb9f8f0300fc69b4bd70d6d61e1f10160777cbd8e80088ca519c2
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57333086"
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
unifiedRoleDefinition.isEnabled = false;

graphClient.roleManagement().directory().roleDefinitions()
    .buildRequest()
    .post(unifiedRoleDefinition);

```