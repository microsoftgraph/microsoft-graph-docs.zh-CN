---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 09be4266fbe8f5d4e456327b43d7d6587eb7b928
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2022
ms.locfileid: "62348634"
---
```powershell

Import-Module Microsoft.Graph.Groups

$params = @{
    Post = @{
        Body = @{
            ContentType = ""
            Content = "content-value"
        }
        ReceivedDateTime = [System.DateTime]::Parse("datetime-value")
        HasAttachments = $true
        From = @{
            EmailAddress = @{
                Name = "name-value"
                Address = "address-value"
            }
        }
        Sender = @{
            EmailAddress = @{
                Name = "name-value"
                Address = "address-value"
            }
        }
        ConversationThreadId = "conversationThreadId-value"
        NewParticipants = @(
            @{
                EmailAddress = @{
                    Name = "name-value"
                    Address = "address-value"
                }
            }
        )
        ConversationId = "conversationId-value"
        CreatedDateTime = [System.DateTime]::Parse("datetime-value")
        LastModifiedDateTime = [System.DateTime]::Parse("datetime-value")
        ChangeKey = "changeKey-value"
        Categories = @(
            "categories-value"
        )
        Id = "id-value"
        InReplyTo = @{
        }
        Attachments = @(
            @{
                "@odata.type" = "#microsoft.graph.fileAttachment"
                LastModifiedDateTime = [System.DateTime]::Parse("datetime-value")
                Name = "name-value"
                ContentType = "contentType-value"
                Size = 99
                IsInline = $true
                Id = "id-value"
            }
        )
    }
}

Invoke-MgReplyGroupThreadPost -GroupId $groupId -ConversationThreadId $conversationThreadId -PostId $postId -BodyParameter $params

```