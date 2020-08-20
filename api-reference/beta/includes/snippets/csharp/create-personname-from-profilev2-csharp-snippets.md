---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 25b9b879e1d0cc09e46e1b174754ba50785af3f3
ms.sourcegitcommit: 239db9e961e42b505f52de9859963a9136935f2f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/20/2020
ms.locfileid: "46821010"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var personName = new PersonName
{
    DisplayName = "Innocenty Popov",
    First = "Innocenty",
    Initials = "IP",
    Last = "Popov",
    LanguageTag = "en-US",
    Maiden = null
};

await graphClient.Me.Profile.Names
    .Request()
    .AddAsync(personName);

```