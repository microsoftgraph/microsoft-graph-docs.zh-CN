---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 688427ba8f00a448cd55441146e524acb7d42536
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59507896"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const bulkReprovisionCloudPc = {
  managedDeviceIds: ['30d0e128-de93-41dc-89ec-33d84bb662a0', '7c82a3e3-9459-44e4-94d9-b92f93bf78dd'] 
};

await client.api('/deviceManagement/managedDevices/bulkReprovisionCloudPc')
    .version('beta')
    .post(bulkReprovisionCloudPc);

```