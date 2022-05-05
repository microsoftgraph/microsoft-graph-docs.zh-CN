---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a154f9e81ed5e30982844c63059e678b2c6d5281
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65202369"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

InternalDomainFederation internalDomainFederation = new InternalDomainFederation();
internalDomainFederation.displayName = "Contoso";
internalDomainFederation.issuerUri = "http://contoso.com/adfs/services/trust";
internalDomainFederation.metadataExchangeUri = "https://sts.contoso.com/adfs/services/trust/mex";
internalDomainFederation.signingCertificate = "MIIE3jCCAsagAwIBAgIQQcyDaZz3MI";
internalDomainFederation.passiveSignInUri = "https://sts.contoso.com/adfs/ls";
internalDomainFederation.preferredAuthenticationProtocol = AuthenticationProtocol.WS_FED;
internalDomainFederation.activeSignInUri = "https://sts.contoso.com/adfs/services/trust/2005/usernamemixed";
internalDomainFederation.signOutUri = "https://sts.contoso.com/adfs/ls";
internalDomainFederation.promptLoginBehavior = PromptLoginBehavior.NATIVE_SUPPORT;
internalDomainFederation.isSignedAuthenticationRequestRequired = true;
internalDomainFederation.nextSigningCertificate = "MIIE3jCCAsagAwIBAgIQQcyDaZz3MI";
internalDomainFederation.federatedIdpMfaBehavior = FederatedIdpMfaBehavior.REJECT_MFA_BY_FEDERATED_IDP;

graphClient.domains("contoso.com").federationConfiguration()
    .buildRequest()
    .post(internalDomainFederation);

```