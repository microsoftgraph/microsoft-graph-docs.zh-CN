---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 85eaa76445399692b8471986f79ee837173c161571d0007e0c7c15f172ce6591
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57164314"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var projectParticipation = new ProjectParticipation
{
    Categories = new List<String>()
    {
        "Branding"
    },
    Client = new CompanyDetail
    {
        DisplayName = "Contoso Ltd.",
        Department = "Corporate Marketing",
        WebUrl = "https://www.contoso.com"
    },
    DisplayName = "Contoso Re-branding Project",
    Detail = new PositionDetail
    {
        Company = new CompanyDetail
        {
            DisplayName = "Adventureworks Inc.",
            Department = "Consulting",
            WebUrl = "https://adventureworks.com"
        },
        Description = "Rebranding of Contoso Ltd.",
        JobTitle = "Lead PM Rebranding",
        Role = "project management",
        Summary = "A 6 month project to help Contoso rebrand after they were divested from a parent organization."
    }
};

await graphClient.Me.Profile.Projects
    .Request()
    .AddAsync(projectParticipation);

```