---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 44851f8a3e93afe4f2021885af6a8a2177f54603
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62113425"
---
```powershell

Import-Module Microsoft.Graph.Groups

$params = @{
    Topic = "New head count"
    Threads = @(
        @{
            Posts = @(
                @{
                    Body = @{
                        ContentType = "html"
                        Content = "The confirmation will come by the end of the week."
                    }
                    NewParticipants = @(
                        @{
                            EmailAddress = @{
                                Name = "Adele Vance"
                                Address = "AdeleV@contoso.onmicrosoft.com"
                            }
                        }
                    )
                }
            )
        }
    )
}

New-MgGroupConversation -GroupId $groupId -BodyParameter $params

```