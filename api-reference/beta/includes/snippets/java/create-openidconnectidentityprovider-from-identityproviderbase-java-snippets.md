---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1a391f604594dc855d71c2135976911a6b9a330a9905f24dfa29aff218646740
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57105745"
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