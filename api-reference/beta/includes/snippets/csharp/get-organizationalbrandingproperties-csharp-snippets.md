---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: fe1db2ad7f06574874b1c8fbf31ec1d34c30cca9
ms.sourcegitcommit: 42fdb068616222eb6b0813e93b33e830fc7eedc0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/17/2021
ms.locfileid: "50274807"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var organizationalBrandingLocalization = new OrganizationalBrandingLocalization
{
    BackgroundColor = "#00000F",
    Id = "fr"
};

await graphClient.Organization["d69179bf-f4a4-41a9-a9de-249c0f2efb1d"].Branding.Localizations
    .Request()
    .AddAsync(organizationalBrandingLocalization);

```