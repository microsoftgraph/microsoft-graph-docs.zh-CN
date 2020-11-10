---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7b6a3450e82cdc6648b33c7e2263eb620ed5defe
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48953377"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

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