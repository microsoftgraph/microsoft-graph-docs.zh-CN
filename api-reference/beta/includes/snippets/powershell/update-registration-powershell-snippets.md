---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a18084ad7164634743c8ab0f52b6eb3ad609881a
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62113167"
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

Update-MgUserOnlineMeetingRegistration -UserId $userId -OnlineMeetingId $onlineMeetingId -BodyParameter $params

```