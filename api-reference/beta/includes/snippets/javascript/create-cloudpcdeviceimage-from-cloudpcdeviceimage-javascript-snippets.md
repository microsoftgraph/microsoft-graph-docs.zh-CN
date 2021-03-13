---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d3a3a6a5db4d74b45e14cffe01e5677cf04c4a9a
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50789186"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const cloudPcDeviceImage = {
  '@odata.type': '#microsoft.graph.cloudPcDeviceImage',
  displayName: 'Display Name value',
  osBuildNumber: 'OS Build Number value',
  operatingSystem: 'Operating System value',
  version: 'Version value',
  sourceImageResourceId: '/subscriptions/0ac520ee-14c0-480f-b6c9-0a90c58ffff/resourceGroups/Example/providers/Microsoft.Compute/images/exampleImage'
};

await client.api('/deviceManagement/virtualEndpoint/deviceImages')
    .version('beta')
    .post(cloudPcDeviceImage);

```