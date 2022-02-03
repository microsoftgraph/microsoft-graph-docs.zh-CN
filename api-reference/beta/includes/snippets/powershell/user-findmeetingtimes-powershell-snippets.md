---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 144b76598f5eab50aadced98c2ada6d218dca846
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2022
ms.locfileid: "62339110"
---
```powershell

Import-Module Microsoft.Graph.Users.Actions

$params = @{
    Attendees = @(
        @{
            Type = "required"
            EmailAddress = @{
                Name = "Alex Wilbur"
                Address = "alexw@contoso.onmicrosoft.com"
            }
        }
    )
    LocationConstraint = @{
        IsRequired = "false"
        SuggestLocation = "false"
        Locations = @(
            @{
                ResolveAvailability = "false"
                DisplayName = "Conf room Hood"
            }
        )
    }
    TimeConstraint = @{
        ActivityDomain = "work"
        TimeSlots = @(
            @{
                Start = @{
                    DateTime = "2019-04-16T09:00:00"
                    TimeZone = "Pacific Standard Time"
                }
                End = @{
                    DateTime = "2019-04-18T17:00:00"
                    TimeZone = "Pacific Standard Time"
                }
            }
        )
    }
    IsOrganizerOptional = "false"
    MeetingDuration = "PT1H"
    ReturnSuggestionReasons = "true"
    MinimumAttendeePercentage = "100"
}

# A UPN can also be used as -UserId.
Find-MgUserMeetingTime -UserId $userId -BodyParameter $params

```