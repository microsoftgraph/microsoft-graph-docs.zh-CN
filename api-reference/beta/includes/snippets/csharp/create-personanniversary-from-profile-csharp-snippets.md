---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 05f714d65c523a681a8ec3a0cceab16fdaef4ff3
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/25/2019
ms.locfileid: "37996580"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var personAnniversary = new PersonAnniversary
{
    Type = AnniversaryType.Birthday,
    Date = new Date(1900,1,1)
};

await graphClient.Me.Profile.Anniversaries
    .Request()
    .AddAsync(personAnniversary);

```