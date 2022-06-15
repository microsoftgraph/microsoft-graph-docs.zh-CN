---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b332b80a2ed2a06ff67f77490201faa024816644
ms.sourcegitcommit: 6bb3c5c043d35476e41ef2790bcf4813fae0769d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/15/2022
ms.locfileid: "66098776"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewShiftPreferences()
id := "SHPR_eeab4fb1-20e5-48ca-ad9b-98119d94bee7"
requestBody.SetId(&id)
requestBody.SetAvailability( []ShiftAvailability {
    msgraphsdk.NewShiftAvailability(),
recurrence := msgraphsdk.NewPatternedRecurrence()
    SetRecurrence(recurrence)
pattern := msgraphsdk.NewRecurrencePattern()
    recurrence.SetPattern(pattern)
type := "Weekly"
    pattern.SetType(&type)
    pattern.SetDaysOfWeek( []DayOfWeek {
        "Monday",
        "Wednesday",
        "Friday",
    }
interval := int32(1)
    pattern.SetInterval(&interval)
range := msgraphsdk.NewRecurrenceRange()
    recurrence.SetRange(range)
type := "noEnd"
    range.SetType(&type)
timeZone := "Pacific Standard Time"
    SetTimeZone(&timeZone)
    SetTimeSlots(nil)
}
requestBody.SetAdditionalData(map[string]interface{}{
    "@odata.etag": "1a371e53-f0a6-4327-a1ee-e3c56e4b38aa",
}
userId := "user-id"
graphClient.UsersById(&userId).Settings().ShiftPreferences().Patch(requestBody)


```