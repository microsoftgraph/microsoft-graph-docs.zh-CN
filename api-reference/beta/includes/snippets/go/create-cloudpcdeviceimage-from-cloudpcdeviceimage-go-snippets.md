---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3600f6e49641786018e94fdb2d93a47738610e00
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61019269"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

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
options := &msgraphsdk.DeviceImagesRequestBuilderPostOptions{
    Body: requestBody,
}
result, err := graphClient.DeviceManagement().VirtualEndpoint().DeviceImages().Post(options)


```