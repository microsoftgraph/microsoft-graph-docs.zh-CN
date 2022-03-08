---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 192393232adeb7013091a4bc7bb76bb6ee6c51a5
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/08/2022
ms.locfileid: "63338873"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const restoreCloudPc = {
  cloudPcSnapshotId: 'A00009UV000_93aff428-61f2-467f-a879-1102af6fd4a8'
};

await client.api('/deviceManagement/managedDevices/5e1387aa-d960-4916-ae7c-293b977e49bf/restoreCloudPc')
    .version('beta')
    .post(restoreCloudPc);

```