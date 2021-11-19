---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 31c7b39e441ad03c3a75e3c9bf2151ceea8ae7cb
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61085273"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewDevice()
extensionAttributes := msgraphsdk.NewOnPremisesExtensionAttributes()
requestBody.SetExtensionAttributes(extensionAttributes)
extensionAttribute1 := "BYOD-Device"
extensionAttributes.SetExtensionAttribute1(&extensionAttribute1)
options := &msgraphsdk.DeviceRequestBuilderPatchOptions{
    Body: requestBody,
}
deviceId := "device-id"
graphClient.DevicesById(&deviceId).Patch(options)


```