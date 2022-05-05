---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 417cf177930e73f38931f14287b00b3deb5f4d18
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65208928"
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
            TeamsAppId = "881b8843-fd91-49e5-9ac2-47ec497ffbe5"
        }
    )
}

New-MgTeamChannelMessage -TeamId $teamId -ChannelId $channelId -BodyParameter $params

```