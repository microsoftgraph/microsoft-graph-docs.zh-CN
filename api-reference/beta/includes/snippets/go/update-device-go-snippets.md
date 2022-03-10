---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2f02d001065b7d8fd834c0babd800d1176717980
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63411678"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewDevice()
accountEnabled := false
requestBody.SetAccountEnabled(&accountEnabled)
options := &msgraphsdk.DeviceRequestBuilderPatchOptions{
    Body: requestBody,
}
deviceId := "device-id"
result, err := graphClient.DevicesById(&deviceId).Patch(options)


```