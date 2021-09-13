---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 16751affff0fd0aa6ca0d785bdb48cc26381db546de33b364779a908645f9b1f
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57333347"
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

await graphClient.Users["{user-id}"].Settings.ShiftPreferences
    .Request()
    .UpdateAsync(shiftPreferences);

```