---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d562658d71b65d47c6d90cb365d33f8f98b3d12d
ms.sourcegitcommit: 82da4012294b046416c9ae93d2294d80dab217f6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/04/2020
ms.locfileid: "48905794"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var certificateBasedAuthConfiguration = new CertificateBasedAuthConfiguration
{
    CertificateAuthorities = new List<CertificateAuthority>()
    {
        new CertificateAuthority
        {
            IsRootAuthority = true,
            Certificate = Encoding.ASCII.GetBytes("Binary")
        }
    }
};

await graphClient.Organization["{id}"].CertificateBasedAuthConfiguration.References
    .Request()
    .AddAsync(certificateBasedAuthConfiguration);

```