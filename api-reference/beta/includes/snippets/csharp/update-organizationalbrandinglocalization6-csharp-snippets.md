---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f56e3331dd30a3cfe428f9e22a30dfeb41382695
ms.sourcegitcommit: 36bae3615df41876493b25da478e589d1974f97b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/29/2021
ms.locfileid: "59996566"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var organizationalBrandingLocalization = new OrganizationalBrandingLocalization
{
    BackgroundColor = "#00000F",
    SignInPageText = "Welcome to Contoso France"
};

await graphClient.Organization["{organization-id}"].Branding.Localizations["{organizationalBrandingLocalization-id}"]
    .Request()
    .UpdateAsync(organizationalBrandingLocalization);

```