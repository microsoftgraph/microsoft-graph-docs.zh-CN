---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c69b639d27920c13a0d815a5ebfa187bf589e72d
ms.sourcegitcommit: 08e9b0bac39c1b1d2c8a79539d24aaa93364baf2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/24/2021
ms.locfileid: "59508653"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var samlOrWsFedExternalDomainFederation = new SamlOrWsFedExternalDomainFederation
{
    DisplayName = "Contoso name change",
    IssuerUri = "http://contoso-test.com/adfs/services/trust",
    MetadataExchangeUri = null,
    SigningCertificate = "M66C6DCCAdCgAwIBAgIQQ6vYJIVKQ",
    PassiveSignInUri = "https://contoso-test.com/adfs/ls/",
    PreferredAuthenticationProtocol = AuthenticationProtocol.WsFed
};

await graphClient.Directory.FederationConfigurations["{samlOrWsFedExternalDomainFederation-id}"]
    .Request()
    .UpdateAsync(samlOrWsFedExternalDomainFederation);

```