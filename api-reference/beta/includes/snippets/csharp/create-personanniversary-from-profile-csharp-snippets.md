---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3d59c6d6eb8d05ad383c90cfa45a8713665deb390b4d19677009c2415f9d094b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57279493"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var personAnnualEvent = new PersonAnnualEvent
{
    Type = PersonAnnualEventType.Birthday,
    Date = new Date(1980,1,8)
};

await graphClient.Me.Profile.Anniversaries
    .Request()
    .AddAsync(personAnnualEvent);

```