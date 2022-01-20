---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: bdc75841341d0fab405944f8c6ff8c7ca8cf0456
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62109454"
---
```powershell

Import-Module Microsoft.Graph.Teams

$params = @{
    Subject = $null
    Body = @{
        ContentType = "html"
        Content = "<attachment id="74d20c7f34aa4a7fb74e2b30004247c5"></attachment>"
    }
    Attachments = @(
        @{
            Id = "74d20c7f34aa4a7fb74e2b30004247c5"
            ContentType = "application/vnd.microsoft.card.thumbnail"
            ContentUrl = $null
            Content = "{
  "title": "This is an example of posting a card",
  "subtitle": "<h3>This is the subtitle</h3>",
  "text": "Here is some body text. <br>\r\nAnd a <a href=\"http://microsoft.com/\">hyperlink</a>. <br>\r\nAnd below that is some buttons:",
  "buttons": [
    {
      "type": "messageBack",
      "title": "Login to FakeBot",
      "text": "login",
      "displayText": "login",
      "value": "login"
    }
  ]
}"
            Name = $null
            ThumbnailUrl = $null
        }
    )
}

New-MgTeamChannelMessage -TeamId $teamId -ChannelId $channelId -BodyParameter $params

```