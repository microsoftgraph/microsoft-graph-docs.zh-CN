---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c3eb8210f36f270020815ca175518a774e735ce7
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65327209"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewShiftPreferences()
id := "SHPR_eeab4fb1-20e5-48ca-ad9b-98119d94bee7"
requestBody.SetId(&id)
requestBody.SetAvailability( []ShiftAvailability {
    msgraphsdk.NewShiftAvailability(),
    SetAdditionalData(map[string]interface{}{
        "timeZone": "Pacific Standard Time",
        "timeSlots": nil,
    }
}
requestBody.SetAdditionalData(map[string]interface{}{
    "@odata.etag": "1a371e53-f0a6-4327-a1ee-e3c56e4b38aa",
}
userId := "user-id"
graphClient.UsersById(&userId).Settings().ShiftPreferences().Patch(requestBody)


```