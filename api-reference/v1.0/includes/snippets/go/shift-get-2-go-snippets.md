---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 39b50c44342aa89fcaf4ab5876d8f3b882f6342b
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "60995944"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

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
graphClient.UsersById(&userId).Settings().ShiftPreferences().Patch(options)


```