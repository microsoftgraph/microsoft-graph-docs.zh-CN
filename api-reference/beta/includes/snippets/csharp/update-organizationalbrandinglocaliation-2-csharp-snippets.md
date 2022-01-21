---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d92c1914a0e4675647a2ca5a957265251736dcde
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62112818"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var stream = new System.IO.MemoryStream(Encoding.UTF8.GetBytes(@"<Image>
"));

var branding = new OrganizationalBranding();
branding.BannerLogo = stream;

await graphClient.Organization["{organization-id}"].Branding
    .Request()
    .UpdateAsync(branding);

```