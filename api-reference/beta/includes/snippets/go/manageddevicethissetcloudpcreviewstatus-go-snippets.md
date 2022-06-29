---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6330e9608ab5b6508987956280d06f639570946a
ms.sourcegitcommit: 54ba08a80db85b9e84813387e8c4416eca44fa8e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/26/2022
ms.locfileid: "65694521"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewReviewStatusRequestBody()
reviewStatus := msgraphsdk.NewCloudPcReviewStatus()
requestBody.SetReviewStatus(reviewStatus)
inReview := true
reviewStatus.SetInReview(&inReview)
userAccessLevel := "restricted"
reviewStatus.SetUserAccessLevel(&userAccessLevel)
azureStorageAccountId := "/subscriptions/f68bd846-16ad-4b51-a7c6-c84944a3367c/resourceGroups/Review/providers/Microsoft.Storage/storageAccounts/snapshotsUnderReview"
reviewStatus.SetAzureStorageAccountId(&azureStorageAccountId)
managedDeviceId := "managedDevice-id"
graphClient.DeviceManagement().ManagedDevicesById(&managedDeviceId).SetCloudPcReviewStatus(managedDevice-id).Post(requestBody)


```