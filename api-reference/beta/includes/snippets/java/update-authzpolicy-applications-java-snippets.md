---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3cdcfdee1ca6d332a21fc8e1812353cb849bcf82e6c4d6abaa94b273102e9fd4
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57105054"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

AuthorizationPolicy authorizationPolicy = new AuthorizationPolicy();
DefaultUserRolePermissions defaultUserRolePermissions = new DefaultUserRolePermissions();
defaultUserRolePermissions.allowedToCreateApps = false;
authorizationPolicy.defaultUserRolePermissions = defaultUserRolePermissions;

graphClient.policies().authorizationPolicy("authorizationPolicy")
    .buildRequest()
    .patch(authorizationPolicy);

```