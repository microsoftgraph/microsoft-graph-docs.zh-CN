---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a908a734e5b2b297be9dd544185bdad1226c1ef0
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61089844"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.New()
requestBody.SetAdditionalData(map[string]interface{}{
    "id": "SHPR_eeab4fb1-20e5-48ca-ad9b-98119d94bee7",
    "@odata.etag": "1a371e53-f0a6-4327-a1ee-e3c56e4b38aa",
    "availability":  []Object {
    }
}
options := &msgraphsdk.ShiftPreferencesRequestBuilderPutOptions{
    Body: requestBody,
}
userId := "user-id"
graphClient.UsersById(&userId).Settings().ShiftPreferences().Put(options)


```