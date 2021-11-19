---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4c9102b0c43dad0da716ae9c0dbe56e7f72a735f
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61084832"
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
graphClient.UsersById(&userId).Settings().ShiftPreferences().Patch(options)


```