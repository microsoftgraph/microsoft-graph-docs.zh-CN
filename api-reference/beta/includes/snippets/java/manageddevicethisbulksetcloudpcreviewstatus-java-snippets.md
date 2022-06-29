---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: bfb798071a6d8d70992c014b3f05311b824c216e
ms.sourcegitcommit: 54ba08a80db85b9e84813387e8c4416eca44fa8e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/26/2022
ms.locfileid: "65695570"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LinkedList<String> managedDeviceIdsList = new LinkedList<String>();
managedDeviceIdsList.add("30d0e128-de93-41dc-89ec-33d84bb662a0");
managedDeviceIdsList.add("7c82a3e3-9459-44e4-94d9-b92f93bf78dd");

CloudPcReviewStatus reviewStatus = new CloudPcReviewStatus();
reviewStatus.inReview = true;
reviewStatus.userAccessLevel = CloudPcUserAccessLevel.RESTRICTED;
reviewStatus.azureStorageAccountId = "/subscriptions/f68bd846-16ad-4b51-a7c6-c84944a3367c/resourceGroups/Review/providers/Microsoft.Storage/storageAccounts/snapshotsUnderReview";

graphClient.deviceManagement().managedDevices()
    .bulkSetCloudPcReviewStatus(ManagedDeviceBulkSetCloudPcReviewStatusParameterSet
        .newBuilder()
        .withManagedDeviceIds(managedDeviceIdsList)
        .withReviewStatus(reviewStatus)
        .build())
    .buildRequest()
    .post();

```