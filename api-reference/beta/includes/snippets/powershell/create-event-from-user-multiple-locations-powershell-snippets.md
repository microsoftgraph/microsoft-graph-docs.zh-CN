---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 11e16a6b25a5b4a58b163df89802e299be0b6a94
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62130599"
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

New-MgUserEvent -UserId $userId -BodyParameter $params

```