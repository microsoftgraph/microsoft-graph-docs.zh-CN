---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f6721be75bf6ea9bb36e840cdb608448da6bb6061d03a0c62575c3b2866e580a
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57278956"
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