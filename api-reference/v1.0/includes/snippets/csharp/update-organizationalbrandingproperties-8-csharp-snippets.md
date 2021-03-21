---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d8112320c1432dcce1584446791044711c4279bd
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50959717"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var organizationalBrandingLocalization = new OrganizationalBrandingLocalization
{
    BackgroundColor = "#00000F",
    SignInPageText = "fr"
};

await graphClient.Organization["{organization-id}"].Branding.Localizations["{organizationalBrandingLocalization-id}"]
    .Request()
    .PutAsync(organizationalBrandingLocalization);

```