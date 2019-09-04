---
description: 自动生成的文件。 不修改
ms.openlocfilehash: a283d07e7c665b13a15d092579b75984126f9e93
ms.sourcegitcommit: d1742ec820776f1e95cba76d98c6cfd17d3eadbb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/04/2019
ms.locfileid: "36720070"
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
            Certificate = "Binary"
        }
    }
};

await graphClient.Organization["{id}"].CertificateBasedAuthConfiguration
    .Request()
    .AddAsync(certificateBasedAuthConfiguration);

```