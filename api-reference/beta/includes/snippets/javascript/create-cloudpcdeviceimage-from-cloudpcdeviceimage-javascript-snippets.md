---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 953dce76cc42a312f199145610c59302fa8a36fc
ms.sourcegitcommit: 9f88b7e41a4a4a4d5f52bd995ce07c6f702bd5d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/01/2020
ms.locfileid: "49523556"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const cloudPcDeviceImage = {
  @odata.type: "#microsoft.graph.cloudPcDeviceImage",
  displayName: "Display Name value",
  osBuildNumber: "OS Build Number value",
  operatingSystem: "Operating System value",
  version: "Version value",
  sourceImageResourceId: "/subscriptions/0ac520ee-14c0-480f-b6c9-0a90c58ffff/resourceGroups/Example/providers/Microsoft.Compute/images/exampleImage"
};

let res = await client.api('/deviceManagement/virtualEndpoint/deviceImages')
    .version('beta')
    .post(cloudPcDeviceImage);

```