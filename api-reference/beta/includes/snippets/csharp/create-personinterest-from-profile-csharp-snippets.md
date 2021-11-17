---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 72b8bf4d6928dbdc98323a46b2aed3a921ccdb29d92c81a9bc1e417535a20911
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57279593"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var personInterest = new PersonInterest
{
    Categories = new List<String>()
    {
        "Sports"
    },
    Description = "World's greatest football club",
    DisplayName = "Chelsea FC",
    WebUrl = "https://www.chelseafc.com"
};

await graphClient.Me.Profile.Interests
    .Request()
    .AddAsync(personInterest);

```