---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4641308799106b6c34c73efba39e2e72c5403862
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50977532"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

OpenIdConnectProvider identityProvider = new OpenIdConnectProvider();
identityProvider.name = "Login with the Contoso identity provider";
identityProvider.type = "OpenIDConnect";
identityProvider.clientId = "56433757-cadd-4135-8431-2c9e3fd68ae8";
identityProvider.clientSecret = "12345";
ClaimsMapping claimsMapping = new ClaimsMapping();
claimsMapping.userId = "myUserId";
claimsMapping.givenName = "myGivenName";
claimsMapping.surname = "mySurname";
claimsMapping.email = "myEmail";
claimsMapping.displayName = "myDisplayName";
identityProvider.claimsMapping = claimsMapping;
identityProvider.domainHint = "mycustomoidc";
identityProvider.metadataUrl = "https://mycustomoidc.com/.well-known/openid-configuration";
identityProvider.responseMode = OpenIdConnectResponseMode.FORM_POST;
identityProvider.responseType = EnumSet.of(OpenIdConnectResponseTypes.CODE);
identityProvider.scope = "openid";

graphClient.identityProviders()
    .buildRequest()
    .post(identityProvider);

```