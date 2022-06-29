---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a4d4d52d00c0871cfae7783913f21848a0d0b2bd
ms.sourcegitcommit: 54ba08a80db85b9e84813387e8c4416eca44fa8e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/26/2022
ms.locfileid: "65694524"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

CloudPcReviewStatus reviewStatus = new CloudPcReviewStatus();
reviewStatus.inReview = true;
reviewStatus.userAccessLevel = CloudPcUserAccessLevel.RESTRICTED;
reviewStatus.azureStorageAccountId = "/subscriptions/f68bd846-16ad-4b51-a7c6-c84944a3367c/resourceGroups/Review/providers/Microsoft.Storage/storageAccounts/snapshotsUnderReview";

graphClient.deviceManagement().managedDevices("185f01c2de954929afb129392e5d9f47")
    .setCloudPcReviewStatus(ManagedDeviceSetCloudPcReviewStatusParameterSet
        .newBuilder()
        .withReviewStatus(reviewStatus)
        .build())
    .buildRequest()
    .post();

```