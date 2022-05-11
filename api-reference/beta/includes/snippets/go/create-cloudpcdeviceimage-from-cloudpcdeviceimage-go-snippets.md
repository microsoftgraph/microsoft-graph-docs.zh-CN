---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d4b1ef1735b50c7ffeb232e023c8296b12af7a0d
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65327659"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewCloudPcDeviceImage()
displayName := "Display Name value"
requestBody.SetDisplayName(&displayName)
osBuildNumber := "OS Build Number value"
requestBody.SetOsBuildNumber(&osBuildNumber)
operatingSystem := "Operating System value"
requestBody.SetOperatingSystem(&operatingSystem)
version := "Version value"
requestBody.SetVersion(&version)
sourceImageResourceId := "/subscriptions/0ac520ee-14c0-480f-b6c9-0a90c58ffff/resourceGroups/Example/providers/Microsoft.Compute/images/exampleImage"
requestBody.SetSourceImageResourceId(&sourceImageResourceId)
requestBody.SetAdditionalData(map[string]interface{}{
    "@odata.type": "#microsoft.graph.cloudPcDeviceImage",
}
result, err := graphClient.DeviceManagement().VirtualEndpoint().DeviceImages().Post(requestBody)


```