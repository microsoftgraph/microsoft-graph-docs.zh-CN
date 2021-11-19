---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8e47ba09afbb717904db024267f881b1f1344bbb
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61088901"
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
options := &msgraphsdk.DevicesRequestBuilderPostOptions{
    Body: requestBody,
}
result, err := graphClient.Devices().Post(options)


```