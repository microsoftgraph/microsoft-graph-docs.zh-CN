---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6aa1f07bc55cf4a926d9396c32f431929445b65b
ms.sourcegitcommit: c650b95ef4d0c3e93e2eb36cd6b52ed31200164f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/10/2020
ms.locfileid: "44684892"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var shiftPreferences = new ShiftPreferences
{
    Id = "SHPR_eeab4fb1-20e5-48ca-ad9b-98119d94bee7",
    Availability = new List<ShiftAvailability>()
    {
        new ShiftAvailability
        {
            Recurrence = new PatternedRecurrence
            {
                Pattern = new RecurrencePattern
                {
                    Type = RecurrencePatternType.Weekly,
                    DaysOfWeek = new List<DayOfWeek>()
                    {
                        DayOfWeek.Monday,
                        DayOfWeek.Wednesday,
                        DayOfWeek.Friday
                    },
                    Interval = 1
                },
                Range = new RecurrenceRange
                {
                    Type = RecurrenceRangeType.NoEnd
                }
            },
            TimeZone = "Pacific Standard Time",
            TimeSlots = null
        }
    },
    AdditionalData = new Dictionary<string, object>()
    {
        {"@odata.etag", "1a371e53-f0a6-4327-a1ee-e3c56e4b38aa"}
    }
};

await graphClient.Users["871dbd5c-3a6a-4392-bfe1-042452793a50"].Settings.ShiftPreferences
    .Request()
    .UpdateAsync(shiftPreferences);

```