---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6e0e4693984ae9eed059776e746fafb4d553385d
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65327857"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewDevice()
accountEnabled := true
requestBody.SetAccountEnabled(&accountEnabled)
requestBody.SetAlternativeSecurityIds( []AlternativeSecurityId {
    msgraphsdk.NewAlternativeSecurityId(),
    SetAdditionalData(map[string]interface{}{
        "type": ,
        "identityProvider": "identityProvider-value",
        "key": "base64Y3YxN2E1MWFlYw==",
    }
}
approximateLastSignInDateTime, err := time.Parse(time.RFC3339, "2016-10-19T10:37:00Z")
requestBody.SetApproximateLastSignInDateTime(&approximateLastSignInDateTime)
deviceId := "deviceId-value"
requestBody.SetDeviceId(&deviceId)
deviceMetadata := "deviceMetadata-value"
requestBody.SetDeviceMetadata(&deviceMetadata)
deviceVersion := int32(99)
requestBody.SetDeviceVersion(&deviceVersion)
result, err := graphClient.Devices().Post(requestBody)


```