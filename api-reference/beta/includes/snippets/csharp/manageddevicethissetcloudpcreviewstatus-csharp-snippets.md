---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: abf8f5bc7726167ecdeb679b6b1ae255032903ec
ms.sourcegitcommit: 54ba08a80db85b9e84813387e8c4416eca44fa8e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/26/2022
ms.locfileid: "65694523"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var reviewStatus = new CloudPcReviewStatus
{
    InReview = true,
    UserAccessLevel = CloudPcUserAccessLevel.Restricted,
    AzureStorageAccountId = "/subscriptions/f68bd846-16ad-4b51-a7c6-c84944a3367c/resourceGroups/Review/providers/Microsoft.Storage/storageAccounts/snapshotsUnderReview"
};

await graphClient.DeviceManagement.ManagedDevices["{managedDevice-id}"]
    .SetCloudPcReviewStatus(reviewStatus)
    .Request()
    .PostAsync();

```