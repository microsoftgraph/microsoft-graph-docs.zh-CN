---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a14451194a0f8ce421110c0cbc0b23431040242ea590b0f7deb07f6d1c4c0c94
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57106596"
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