---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e61618aa29bac5271e08b7c50a54059ff2bb8cb5
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2022
ms.locfileid: "62349794"
---
```powershell

Import-Module Microsoft.Graph.Calendar

$params = @{
    Subject = "Plan summer company picnic"
    Body = @{
        ContentType = "HTML"
        Content = "Let's kick-start this event planning!"
    }
    Start = @{
        DateTime = "2017-08-30T11:00:00"
        TimeZone = "Pacific Standard Time"
    }
    End = @{
        DateTime = "2017-08-30T12:00:00"
        TimeZone = "Pacific Standard Time"
    }
    Attendees = @(
        @{
            EmailAddress = @{
                Address = "DanaS@contoso.onmicrosoft.com"
                Name = "Dana Swope"
            }
            Type = "Required"
        }
        @{
            EmailAddress = @{
                Address = "AlexW@contoso.onmicrosoft.com"
                Name = "Alex Wilber"
            }
            Type = "Required"
        }
    )
    Location = @{
        DisplayName = "Conf Room 3; Fourth Coffee; Home Office"
        LocationType = "Default"
    }
    Locations = @(
        @{
            DisplayName = "Conf Room 3"
        }
        @{
            DisplayName = "Fourth Coffee"
            Address = @{
                Street = "4567 Main St"
                City = "Redmond"
                State = "WA"
                CountryOrRegion = "US"
                PostalCode = "32008"
            }
            Coordinates = @{
                Latitude = 47.672
                Longitude = -102.103
            }
        }
        @{
            DisplayName = "Home Office"
        }
    )
    AllowNewTimeProposals = $true
}

# A UPN can also be used as -UserId.
New-MgUserEvent -UserId $userId -BodyParameter $params

```