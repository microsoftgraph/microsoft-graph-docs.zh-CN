---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 792b6e6cedfbfb6be771c8e89589bb165277627a
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65315728"
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