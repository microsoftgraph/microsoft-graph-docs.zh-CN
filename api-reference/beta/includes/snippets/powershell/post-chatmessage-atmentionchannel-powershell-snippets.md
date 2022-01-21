---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5d5271980238bcdad4f0487fa407a35b82bd33df
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62109449"
---
```powershell

Import-Module Microsoft.Graph.Teams

$params = @{
    Body = @{
        ContentType = "html"
        Content = "<div><div><at id="0">General</at>&nbsp;Hello there!</div></div>"
    }
    Mentions = @(
        @{
            Id = 0
            MentionText = "General"
            Mentioned = @{
                Conversation = @{
                    Id = "19:0b50940236084d258c97b21bd01917b0@thread.skype"
                    DisplayName = "General"
                    ConversationIdentityType = "channel"
                }
            }
        }
    )
}

New-MgTeamChannelMessage -TeamId $teamId -ChannelId $channelId -BodyParameter $params

```