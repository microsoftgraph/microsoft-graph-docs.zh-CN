---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7a609dae7775e987ff3f5787ecd65f58c3f2f80f12f97de05885102771861f10
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57163781"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var personWebsite = new PersonWebsite
{
    Categories = new List<String>()
    {
        "football"
    },
    DisplayName = "Lyn Damer",
    WebUrl = "www.lyndamer.no"
};

await graphClient.Me.Profile.Websites
    .Request()
    .AddAsync(personWebsite);

```