---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5e0f0f29689dc76b75bc01cbe4b2c7d8509ca22c
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/29/2022
ms.locfileid: "66444626"
---
```powershell

Import-Module Microsoft.Graph.DeviceManagement.Actions

$params = @{
    ReviewStatus = @{
        InReview = $true
        UserAccessLevel = "restricted"
        AzureStorageAccountId = "/subscriptions/f68bd846-16ad-4b51-a7c6-c84944a3367c/resourceGroups/Review/providers/Microsoft.Storage/storageAccounts/snapshotsUnderReview"
    }
}

Set-MgDeviceManagementManagedDeviceCloudPcReviewStatus -ManagedDeviceId $managedDeviceId -BodyParameter $params

```