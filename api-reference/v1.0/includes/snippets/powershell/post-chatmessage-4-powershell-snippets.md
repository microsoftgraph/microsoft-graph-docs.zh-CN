---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ba86c82b07086c6bcd98ecfd9f09be5c8a7630e5
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62129090"
---
```powershell

Import-Module Microsoft.Graph.Teams

$params = @{
    Body = @{
        ContentType = "html"
        Content = "Here's the latest budget. <attachment id="153fa47d-18c9-4179-be08-9879815a9f90"></attachment>"
    }
    Attachments = @(
        @{
            Id = "153fa47d-18c9-4179-be08-9879815a9f90"
            ContentType = "reference"
            ContentUrl = "https://m365x987948.sharepoint.com/sites/test/Shared%20Documents/General/test%20doc.docx"
            Name = "Budget.docx"
        }
    )
}

New-MgTeamChannelMessage -TeamId $teamId -ChannelId $channelId -BodyParameter $params

```