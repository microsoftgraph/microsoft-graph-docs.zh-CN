---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 64d76e993f71b15c89520ecdf396127d1f6f7dfc
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65327537"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewTargetServicePlanIdRequestBody()
targetServicePlanId := "30d0e128-de93-41dc-89ec-33d84bb662a0"
requestBody.SetTargetServicePlanId(&targetServicePlanId)
managedDeviceId := "managedDevice-id"
graphClient.DeviceManagement().ManagedDevicesById(&managedDeviceId).ResizeCloudPc(managedDevice-id).Post(requestBody)


```