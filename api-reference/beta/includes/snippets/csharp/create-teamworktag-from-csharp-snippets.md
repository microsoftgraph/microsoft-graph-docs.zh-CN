---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6f4f1ae92b05bf4894f1064d1b864767b411743b
ms.sourcegitcommit: 7f674112f5b95446fac86d829509f889c60f1693
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/30/2021
ms.locfileid: "53210034"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var teamworkTag = new TeamworkTag
{
    DisplayName = "Finance",
    Members = new TeamworkTagMembersCollectionPage()
    {
        new TeamworkTagMember
        {
            UserId = "92f6952f-61ca-4a94-8910-508a240bc167"
        },
        new TeamworkTagMember
        {
            UserId = "085d800c-b86b-4bfc-a857-9371ad1caf29"
        }
    }
};

await graphClient.Teams["{team-id}"].Tags
    .Request()
    .AddAsync(teamworkTag);

```