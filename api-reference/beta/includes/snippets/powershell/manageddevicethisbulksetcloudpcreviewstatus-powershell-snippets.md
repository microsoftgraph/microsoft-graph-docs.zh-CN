---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f6cbabb5a03418fee88822d21f491548ff6619b1
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/29/2022
ms.locfileid: "66437183"
---
```powershell

Import-Module Microsoft.Graph.DeviceManagement.Actions

$params = @{
    ManagedDeviceIds = @(
        "30d0e128-de93-41dc-89ec-33d84bb662a0"
        "7c82a3e3-9459-44e4-94d9-b92f93bf78dd"
    )
    ReviewStatus = @{
        InReview = $true
        UserAccessLevel = "restricted"
        AzureStorageAccountId = "/subscriptions/f68bd846-16ad-4b51-a7c6-c84944a3367c/resourceGroups/Review/providers/Microsoft.Storage/storageAccounts/snapshotsUnderReview"
    }
}

Invoke-MgBulkDeviceManagementManagedDeviceSetCloudPcReviewStatus -BodyParameter $params

```