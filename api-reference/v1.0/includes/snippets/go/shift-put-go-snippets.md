---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 605fa1afa8075d4f93660765f889bf76f761080d
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63411985"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.New()
requestBody.SetAdditionalData(map[string]interface{}{
    "id": "SHFT_577b75d2-a927-48c0-a5d1-dc984894e7b8",
    "createdDateTime": "2019-03-14T04:32:51.451Z",
    "lastModifiedDateTime": "2019-03-14T05:32:51.451Z",
    "userId": "c5d0c76b-80c4-481c-be50-923cd8d680a1",
    "schedulingGroupId": "TAG_228940ed-ff84-4e25-b129-1b395cf78be0",
}
headers := map[string]string{
    "Prefer": "return=representation"
}
options := &msgraphsdk.ShiftRequestBuilderPutOptions{
    Body: requestBody,
    H: headers,
}
teamId := "team-id"
shiftId := "shift-id"
graphClient.TeamsById(&teamId).Schedule().ShiftsById(&shiftId).Put(options)


```