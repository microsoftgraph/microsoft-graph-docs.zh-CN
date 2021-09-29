---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d92c1914a0e4675647a2ca5a957265251736dcde
ms.sourcegitcommit: 36bae3615df41876493b25da478e589d1974f97b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/29/2021
ms.locfileid: "59995341"
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