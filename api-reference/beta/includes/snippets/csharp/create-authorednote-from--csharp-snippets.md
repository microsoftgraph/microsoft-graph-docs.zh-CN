---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4246d54b98fb8df3a4e8ff43635ab76e18dae98a
ms.sourcegitcommit: 54ba08a80db85b9e84813387e8c4416eca44fa8e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/26/2022
ms.locfileid: "65719198"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var authoredNote = new AuthoredNote
{
    Content = new ItemBody
    {
        Content = "Please take a look at the files tagged with follow up",
        ContentType = BodyType.Text
    }
};

await graphClient.Privacy.SubjectRightsRequests["{subjectRightsRequest-id}"].Notes
    .Request()
    .AddAsync(authoredNote);

```