---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ecb1ee044f40247c02b2546cd271885d680b9abc
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62109455"
---
```powershell

Import-Module Microsoft.Graph.Teams

$params = @{
    Body = @{
        ContentType = "html"
        Content = "<div><div><at id="0">TestTag</at>&nbsp;Testing Tags</div></div>"
    }
    Mentions = @(
        @{
            Id = 0
            MentionText = "TestTag"
            Mentioned = @{
                Tag = @{
                    Id = "MjQzMmI1N2ItMGFiZC00M2RiLWFhN2ItMTZlYWRkMTE1ZDM0IyM2OGEzZTM2NS1mN2Q5LTRhNTYtYjQ5OS0yNDMzMmE5Y2M1NzIjI3RTMERJZ1Z1ZQ=="
                    DisplayName = "TestTag"
                }
            }
        }
    )
}

New-MgTeamChannelMessage -TeamId $teamId -ChannelId $channelId -BodyParameter $params

```