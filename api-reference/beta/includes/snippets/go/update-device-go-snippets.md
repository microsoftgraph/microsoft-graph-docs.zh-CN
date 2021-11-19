---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f4ebe347ae3f8c6ef85dbc7fd71c7ec54e89315f
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61088137"
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
graphClient.DevicesById(&deviceId).Patch(options)


```