---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f6fbcc6178bd9bc4af57c7f47fed0975d12bf5a4
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61023974"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

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
options := &msgraphsdk.DevicesRequestBuilderPostOptions{
    Body: requestBody,
}
result, err := graphClient.Devices().Post(options)


```