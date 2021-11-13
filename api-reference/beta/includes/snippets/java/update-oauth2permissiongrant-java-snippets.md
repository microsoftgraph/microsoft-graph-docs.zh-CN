---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: aa63d0c1aeaeacfa6ef747a16cd2d4a0f618445eeeacd112ef31becbdea72fda
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57158509"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

OAuth2PermissionGrant oAuth2PermissionGrant = new OAuth2PermissionGrant();
oAuth2PermissionGrant.scope = "scope-value";

graphClient.oauth2PermissionGrants("{id}")
    .buildRequest()
    .patch(oAuth2PermissionGrant);

```