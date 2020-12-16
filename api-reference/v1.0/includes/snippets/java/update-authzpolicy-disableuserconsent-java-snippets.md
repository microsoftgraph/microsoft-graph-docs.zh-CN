---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ade911bf7af689d096595a5477eb00593d89d608
ms.sourcegitcommit: 75428fc7535662f34e965c6b69fef3a53fdaf1cb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/16/2020
ms.locfileid: "49691375"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

AuthorizationPolicy authorizationPolicy = new AuthorizationPolicy();
DefaultUserRolePermissions defaultUserRolePermissions = new DefaultUserRolePermissions();
LinkedList<String> permissionGrantPoliciesAssignedList = new LinkedList<String>();
defaultUserRolePermissions.permissionGrantPoliciesAssigned = permissionGrantPoliciesAssignedList;
authorizationPolicy.defaultUserRolePermissions = defaultUserRolePermissions;

graphClient.policies().authorizationPolicy()
    .buildRequest()
    .patch(authorizationPolicy);

```