---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1042703b86f8dc2dba8e8888bc625e45cd4abaae
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62136084"
---
```powershell

Import-Module Microsoft.Graph.Groups

$params = @{
    Topic = "Take your wellness days and rest"
    Threads = @(
        @{
            Posts = @(
                @{
                    Body = @{
                        ContentType = "html"
                        Content = "Contoso cares about you: Rest and Recharge"
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