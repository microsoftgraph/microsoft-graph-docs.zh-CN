---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ccda3157d4105db5d6cda03c922511de8e176c4c
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65328342"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewDevice()
accountEnabled := false
requestBody.SetAccountEnabled(&accountEnabled)
requestBody.SetAlternativeSecurityIds( []AlternativeSecurityId {
    msgraphsdk.NewAlternativeSecurityId(),
    SetAdditionalData(map[string]interface{}{
        "type": ,
        "key": "base64Y3YxN2E1MWFlYw==",
    }
}
deviceId := "4c299165-6e8f-4b45-a5ba-c5d250a707ff"
requestBody.SetDeviceId(&deviceId)
displayName := "Test device"
requestBody.SetDisplayName(&displayName)
operatingSystem := "linux"
requestBody.SetOperatingSystem(&operatingSystem)
operatingSystemVersion := "1"
requestBody.SetOperatingSystemVersion(&operatingSystemVersion)
result, err := graphClient.Devices().Post(requestBody)


```