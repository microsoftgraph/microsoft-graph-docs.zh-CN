---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0d5b344b222d477feb55d7305fd4bbd1a2e1b95e
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63412550"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewCloudPcSnapshotIdRequestBody()
cloudPcSnapshotId := "A00009UV000_93aff428-61f2-467f-a879-1102af6fd4a8"
requestBody.SetCloudPcSnapshotId(&cloudPcSnapshotId)
options := &msgraphsdk.RestoreCloudPcRequestBuilderPostOptions{
    Body: requestBody,
}
managedDeviceId := "managedDevice-id"
graphClient.DeviceManagement().ManagedDevicesById(&managedDeviceId).RestoreCloudPc(managedDevice-id).Post(options)


```