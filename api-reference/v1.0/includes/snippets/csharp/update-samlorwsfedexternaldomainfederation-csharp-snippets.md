---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c69b639d27920c13a0d815a5ebfa187bf589e72d
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65315250"
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