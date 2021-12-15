---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f82018f8567d3db474fbe0c20a08e112dc4aae9e
ms.sourcegitcommit: c47e3d1f3c5f7e2635b2ad29dfef8fe7c8080bc8
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/15/2021
ms.locfileid: "61525887"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.New()
targetServicePlanId := "30d0e128-de93-41dc-89ec-33d84bb662a0"
requestBody.SetTargetServicePlanId(&targetServicePlanId)
options := &msgraphsdk.ResizeCloudPcRequestBuilderPostOptions{
    Body: requestBody,
}
managedDeviceId := "managedDevice-id"
graphClient.DeviceManagement().ManagedDevicesById(&managedDeviceId).ResizeCloudPc().Post(options)


```