---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4a2ce811583d94cdf6ba69725b36e049f6b2e8d0
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63412105"
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
options := &msgraphsdk.ShiftPreferencesRequestBuilderPatchOptions{
    Body: requestBody,
}
userId := "user-id"
result, err := graphClient.UsersById(&userId).Settings().ShiftPreferences().Patch(options)


```