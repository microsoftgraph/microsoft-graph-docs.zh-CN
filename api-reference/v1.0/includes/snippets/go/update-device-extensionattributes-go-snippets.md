---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f09ce563ff205a480be9113465597db7553b3675
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63412458"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewDevice()
requestBody.SetAdditionalData(map[string]interface{}{
}
options := &msgraphsdk.DeviceRequestBuilderPatchOptions{
    Body: requestBody,
}
deviceId := "device-id"
result, err := graphClient.DevicesById(&deviceId).Patch(options)


```