---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 50bc1ad1bca9ec26370d62c8ed0e9a61c3ce0e21
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50973552"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

OAuth2PermissionGrant oAuth2PermissionGrant = new OAuth2PermissionGrant();
oAuth2PermissionGrant.scope = "scope-value";

graphClient.oauth2PermissionGrants("{id}")
    .buildRequest()
    .patch(oAuth2PermissionGrant);

```