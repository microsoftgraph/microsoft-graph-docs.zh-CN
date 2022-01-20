---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c1d2cef112dbfb6312f66db03b7b4f26f896fdf9
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62136070"
---
```powershell

Import-Module Microsoft.Graph.Calendar

$params = @{
    Subject = "Let's go for lunch"
    Body = @{
        ContentType = "HTML"
        Content = "Does late morning work for you?"
    }
    Start = @{
        DateTime = "2019-06-16T12:00:00"
        TimeZone = "Pacific Standard Time"
    }
    End = @{
        DateTime = "2019-06-16T14:00:00"
        TimeZone = "Pacific Standard Time"
    }
    Location = @{
        DisplayName = "Harry's Bar"
    }
    Attendees = @(
        @{
            EmailAddress = @{
                Address = "adelev@contoso.onmicrosoft.com"
                Name = "Adele Vance"
            }
            Type = "required"
        }
    )
}

New-MgGroupEvent -GroupId $groupId -BodyParameter $params

```