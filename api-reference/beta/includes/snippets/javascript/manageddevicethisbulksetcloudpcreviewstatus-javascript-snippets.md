---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e68d72f737fe401c2a66f50586df5cdf1b11cd04
ms.sourcegitcommit: 54ba08a80db85b9e84813387e8c4416eca44fa8e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/26/2022
ms.locfileid: "65695571"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const cloudPcBulkRemoteActionResult = {
  managedDeviceIds: [
    '30d0e128-de93-41dc-89ec-33d84bb662a0',
    '7c82a3e3-9459-44e4-94d9-b92f93bf78dd'
  ],
  reviewStatus: {
    inReview: true,
    userAccessLevel: 'restricted',
    azureStorageAccountId: '/subscriptions/f68bd846-16ad-4b51-a7c6-c84944a3367c/resourceGroups/Review/providers/Microsoft.Storage/storageAccounts/snapshotsUnderReview'
  }
};

await client.api('/deviceManagement/managedDevices/bulkSetCloudPcReviewStatus')
    .version('beta')
    .post(cloudPcBulkRemoteActionResult);

```