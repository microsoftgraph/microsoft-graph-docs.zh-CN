---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: db062f60f936de4db0c39f2144c543c65439023e
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61096078"
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
options := &msgraphsdk.DevicesRequestBuilderPostOptions{
    Body: requestBody,
}
result, err := graphClient.Devices().Post(options)


```