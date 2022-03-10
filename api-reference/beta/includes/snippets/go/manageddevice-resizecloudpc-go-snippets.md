---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: decd8aa8834c9f6364a8e5dd5b70a835bfc51765
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63412585"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewTargetServicePlanIdRequestBody()
targetServicePlanId := "30d0e128-de93-41dc-89ec-33d84bb662a0"
requestBody.SetTargetServicePlanId(&targetServicePlanId)
options := &msgraphsdk.ResizeCloudPcRequestBuilderPostOptions{
    Body: requestBody,
}
managedDeviceId := "managedDevice-id"
graphClient.DeviceManagement().ManagedDevicesById(&managedDeviceId).ResizeCloudPc(managedDevice-id).Post(options)


```