---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 10c2c535302d1d752955b3d6d774a7e46c632565
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/08/2022
ms.locfileid: "63338189"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.New()
requestBody.SetManagedDeviceIds( []String {
    "30d0e128-de93-41dc-89ec-33d84bb662a0",
    "7c82a3e3-9459-44e4-94d9-b92f93bf78dd",
}
restorePointDateTime, err := time.Parse(time.RFC3339, "2021-09-23T04:00:00.0000000")
requestBody.SetRestorePointDateTime(&restorePointDateTime)
timeRange := "before"
requestBody.SetTimeRange(&timeRange)
options := &msgraphsdk.BulkRestoreCloudPcRequestBuilderPostOptions{
    Body: requestBody,
}
result, err := graphClient.DeviceManagement().ManagedDevices().BulkRestoreCloudPc().Post(options)


```