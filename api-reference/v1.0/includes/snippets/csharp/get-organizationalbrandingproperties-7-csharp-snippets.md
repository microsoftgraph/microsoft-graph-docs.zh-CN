---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ae5619795961874f5343a1c8b070279f08088a0e05f69b3ed768a2dcac907c7b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57162022"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var organizationalBrandingLocalization = new OrganizationalBrandingLocalization
{
    BackgroundColor = "#00000F",
    Id = "fr"
};

await graphClient.Organization["{organization-id}"].Branding.Localizations
    .Request()
    .AddAsync(organizationalBrandingLocalization);

```