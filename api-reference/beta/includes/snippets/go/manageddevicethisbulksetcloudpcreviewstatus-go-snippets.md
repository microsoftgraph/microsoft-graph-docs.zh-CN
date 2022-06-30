---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2c7d0fa2055b6b9c01af2d059037a9b4752e853f
ms.sourcegitcommit: 54ba08a80db85b9e84813387e8c4416eca44fa8e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/26/2022
ms.locfileid: "65695569"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.New()
requestBody.SetManagedDeviceIds( []String {
    "30d0e128-de93-41dc-89ec-33d84bb662a0",
    "7c82a3e3-9459-44e4-94d9-b92f93bf78dd",
}
reviewStatus := msgraphsdk.NewCloudPcReviewStatus()
requestBody.SetReviewStatus(reviewStatus)
inReview := true
reviewStatus.SetInReview(&inReview)
userAccessLevel := "restricted"
reviewStatus.SetUserAccessLevel(&userAccessLevel)
azureStorageAccountId := "/subscriptions/f68bd846-16ad-4b51-a7c6-c84944a3367c/resourceGroups/Review/providers/Microsoft.Storage/storageAccounts/snapshotsUnderReview"
reviewStatus.SetAzureStorageAccountId(&azureStorageAccountId)
result, err := graphClient.DeviceManagement().ManagedDevices().BulkSetCloudPcReviewStatus().Post(requestBody)


```