---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5b9215928a66ff1ffcd3a953db10797cf088bad7c1bc5dc0c048ba04ea875fd0
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57279167"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

using var stream = new System.IO.MemoryStream(Encoding.UTF8.GetBytes(@"<Image>"));

await graphClient.Organization["{organization-id}"].Branding.Localizations["{organizationalBrandingLocalization-id}"].BannerLogo
    .Request()
    .PutAsync<OrganizationalBrandingLocalization>(stream);

```