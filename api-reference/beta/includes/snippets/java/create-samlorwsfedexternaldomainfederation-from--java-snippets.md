---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 792b6e6cedfbfb6be771c8e89589bb165277627a
ms.sourcegitcommit: 08e9b0bac39c1b1d2c8a79539d24aaa93364baf2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/24/2021
ms.locfileid: "59766867"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

SamlOrWsFedExternalDomainFederation identityProviderBase = new SamlOrWsFedExternalDomainFederation();
identityProviderBase.issuerUri = "https://contoso.com/issuerUri";
identityProviderBase.displayName = "contoso display name";
identityProviderBase.metadataExchangeUri = "https://contoso.com/metadataExchangeUri";
identityProviderBase.passiveSignInUri = "https://contoso.com/signin";
identityProviderBase.preferredAuthenticationProtocol = AuthenticationProtocol.WS_FED;
LinkedList<ExternalDomainName> domainsList = new LinkedList<ExternalDomainName>();
ExternalDomainName domains = new ExternalDomainName();
domains.id = "contoso.com";
domainsList.add(domains);
ExternalDomainNameCollectionResponse externalDomainNameCollectionResponse = new ExternalDomainNameCollectionResponse();
externalDomainNameCollectionResponse.value = domainsList;
ExternalDomainNameCollectionPage externalDomainNameCollectionPage = new ExternalDomainNameCollectionPage(externalDomainNameCollectionResponse, null);
identityProviderBase.domains = externalDomainNameCollectionPage;
identityProviderBase.signingCertificate = "MIIDADCCAeigAwIBAgIQEX41y8r6";

graphClient.directory().federationConfigurations()
    .buildRequest()
    .post(identityProviderBase);

```