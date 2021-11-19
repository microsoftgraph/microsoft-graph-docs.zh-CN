---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f5d7254f1eaf18cfca0d0d094c81e5507501f4b1
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61084550"
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
options := &msgraphsdk.DeviceImagesRequestBuilderPostOptions{
    Body: requestBody,
}
result, err := graphClient.DeviceManagement().VirtualEndpoint().DeviceImages().Post(options)


```