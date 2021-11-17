---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 57f0d20fb8a5a23a6754ab36cf0967100c383802d64feda82afcad83cd97fe28
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57105056"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

AuthorizationPolicy authorizationPolicy = new AuthorizationPolicy();
LinkedList<String> permissionGrantPolicyIdsAssignedToDefaultUserRoleList = new LinkedList<String>();
permissionGrantPolicyIdsAssignedToDefaultUserRoleList.add("managePermissionGrantsForSelf.microsoft-user-default-low");
authorizationPolicy.permissionGrantPolicyIdsAssignedToDefaultUserRole = permissionGrantPolicyIdsAssignedToDefaultUserRoleList;

graphClient.policies().authorizationPolicy("authorizationPolicy")
    .buildRequest()
    .patch(authorizationPolicy);

```