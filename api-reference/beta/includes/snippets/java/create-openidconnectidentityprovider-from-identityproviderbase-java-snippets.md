---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9e820a93073e072da1e8789d0d289abf5e6399ca
ms.sourcegitcommit: 32c83957ee69f21a10cd5f759adb884ce4b41c52
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/21/2021
ms.locfileid: "51921325"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

OpenIdConnectIdentityProvider identityProviderBase = new OpenIdConnectIdentityProvider();
identityProviderBase.displayName = "Login with the Contoso identity provider";
identityProviderBase.clientId = "56433757-cadd-4135-8431-2c9e3fd68ae8";
identityProviderBase.clientSecret = "12345";
ClaimsMapping claimsMapping = new ClaimsMapping();
claimsMapping.userId = "myUserId";
claimsMapping.givenName = "myGivenName";
claimsMapping.surname = "mySurname";
claimsMapping.email = "myEmail";
claimsMapping.displayName = "myDisplayName";
identityProviderBase.claimsMapping = claimsMapping;
identityProviderBase.domainHint = "mycustomoidc";
identityProviderBase.metadataUrl = "https://mycustomoidc.com/.well-known/openid-configuration";
identityProviderBase.responseMode = OpenIdConnectResponseMode.FORM_POST;
identityProviderBase.responseType = EnumSet.of(OpenIdConnectResponseTypes.CODE);
identityProviderBase.scope = "openid";

graphClient.identity().identityProviders()
    .buildRequest()
    .post(identityProviderBase);

```