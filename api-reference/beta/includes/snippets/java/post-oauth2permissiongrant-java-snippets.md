---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ffb1ecdbadcebb4489916222a426920101e0d49e
ms.sourcegitcommit: 0d6d39dd6450e0c5fd6844cb78aead00a0782e46
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2022
ms.locfileid: "63758901"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

OAuth2PermissionGrant oAuth2PermissionGrant = new OAuth2PermissionGrant();
oAuth2PermissionGrant.clientId = "ef969797-201d-4f6b-960c-e9ed5f31dab5";
oAuth2PermissionGrant.consentType = "AllPrincipals";
oAuth2PermissionGrant.resourceId = "943603e4-e787-4fe9-93d1-e30f749aae39";
oAuth2PermissionGrant.scope = "DelegatedPermissionGrant.ReadWrite.All";
oAuth2PermissionGrant.startTime = OffsetDateTimeSerializer.deserialize("2022-03-17T00:00:00Z");
oAuth2PermissionGrant.expiryTime = OffsetDateTimeSerializer.deserialize("2023-03-17T00:00:00Z");

graphClient.oauth2PermissionGrants()
    .buildRequest()
    .post(oAuth2PermissionGrant);

```