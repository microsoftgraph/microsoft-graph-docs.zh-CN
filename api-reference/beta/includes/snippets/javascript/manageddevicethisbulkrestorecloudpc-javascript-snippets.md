---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9cf1f6dae7b27b93f438e0f1be53451d6797edf9
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/08/2022
ms.locfileid: "63338194"
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
  restorePointDateTime: '2021-09-23T04:00:00.0000000',
  timeRange: 'before'
};

await client.api('/deviceManagement/managedDevices/bulkRestoreCloudPc')
    .version('beta')
    .post(cloudPcBulkRemoteActionResult);

```