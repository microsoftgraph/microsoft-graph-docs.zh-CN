---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f9feda74b1cd1d8e4d43d2188014f186e357570a
ms.sourcegitcommit: 239db9e961e42b505f52de9859963a9136935f2f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/20/2020
ms.locfileid: "46820200"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var personAnnotation = new PersonAnnotation
{
    Detail = new ItemBody
    {
        ContentType = BodyType.Text,
        Content = "I am originally from Australia, but grew up in Moscow, Russia."
    },
    DisplayName = "About Me"
};

await graphClient.Me.Profile.Notes
    .Request()
    .AddAsync(personAnnotation);

```