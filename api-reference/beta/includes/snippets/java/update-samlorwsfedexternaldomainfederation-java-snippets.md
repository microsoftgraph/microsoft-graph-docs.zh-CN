---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c49a1e21f26fb8e3b231fd49b7f320a9e2d60d97
ms.sourcegitcommit: 08e9b0bac39c1b1d2c8a79539d24aaa93364baf2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/24/2021
ms.locfileid: "59508648"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

SamlOrWsFedExternalDomainFederation samlOrWsFedExternalDomainFederation = new SamlOrWsFedExternalDomainFederation();
samlOrWsFedExternalDomainFederation.displayName = "Contoso name change";
samlOrWsFedExternalDomainFederation.issuerUri = "http://contoso-test.com/adfs/services/trust";
samlOrWsFedExternalDomainFederation.metadataExchangeUri = null;
samlOrWsFedExternalDomainFederation.signingCertificate = "M66C6DCCAdCgAwIBAgIQQ6vYJIVKQ";
samlOrWsFedExternalDomainFederation.passiveSignInUri = "https://contoso-test.com/adfs/ls/";
samlOrWsFedExternalDomainFederation.preferredAuthenticationProtocol = AuthenticationProtocol.WS_FED;

graphClient.directory().federationConfigurations().graph.samlOrWsFedExternalDomainFederation("d5a56845-6845-d5a5-4568-a5d54568a5d5")
    .buildRequest()
    .patch(samlOrWsFedExternalDomainFederation);

```