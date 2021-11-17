---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: fe51295de8496681f9dcfbff93fbe1311811ae5a20e4c07924bd696c5647aee1
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56903049"
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
    .PutAsync(shiftPreferences);

```