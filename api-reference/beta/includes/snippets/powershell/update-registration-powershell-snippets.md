---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8ba05d3f7b527d642fa7e3fc819616252125d881
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2022
ms.locfileid: "62349404"
---
```powershell

Import-Module Microsoft.Graph.CloudCommunications

$params = @{
    Subject = "Microsoft Ignite: Day 1"
    StartDateTime = [System.DateTime]::Parse("2021-11-02T08:00:00-08:00")
    EndDateTime = [System.DateTime]::Parse("2021-11-02T15:45:00-08:00")
    Speakers = @(
        @{
            DisplayName = "Henry Ross"
            Bio = "Chairman and Chief Executive Officer"
        }
        @{
            DisplayName = "Fred Ryan"
            Bio = "CVP"
        }
    )
}

# A UPN can also be used as -UserId.
Update-MgUserOnlineMeetingRegistration -UserId $userId -OnlineMeetingId $onlineMeetingId -BodyParameter $params

```