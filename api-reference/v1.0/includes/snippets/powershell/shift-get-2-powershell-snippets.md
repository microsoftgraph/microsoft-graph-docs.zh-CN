---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b172f656ad9f614e1fff45c6d742c3caba651f42
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62121861"
---
```powershell

Import-Module Microsoft.Graph.Users

$params = @{
    Id = "SHPR_eeab4fb1-20e5-48ca-ad9b-98119d94bee7"
    "@odata.etag" = "1a371e53-f0a6-4327-a1ee-e3c56e4b38aa"
    Availability = @(
        @{
            Recurrence = @{
                Pattern = @{
                    Type = "Weekly"
                    DaysOfWeek = @(
                        "Monday"
                        "Wednesday"
                        "Friday"
                    )
                    Interval = 1
                }
                Range = @{
                    Type = "noEnd"
                }
            }
            TimeZone = "Pacific Standard Time"
            TimeSlots = $null
        }
    )
}

Update-MgUserSettingShiftPreference -UserId $userId -BodyParameter $params

```