---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 975f36d9443e677fa9e35dfa0ca884c9e6760cc35cbf7f573edb23648fc00da5
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57277497"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

OAuth2PermissionGrant oAuth2PermissionGrant = new OAuth2PermissionGrant();
oAuth2PermissionGrant.clientId = "clientId-value";
oAuth2PermissionGrant.consentType = "consentType-value";
oAuth2PermissionGrant.principalId = "principalId-value";
oAuth2PermissionGrant.resourceId = "resourceId-value";
oAuth2PermissionGrant.scope = "scope-value";

graphClient.oauth2PermissionGrants()
    .buildRequest()
    .post(oAuth2PermissionGrant);

```