---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6103d13eb3296e715f6952e4298fcfbae6ac98d5
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50790146"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const device = {
  accountEnabled: false,
  alternativeSecurityIds: 
  [
    {
      type: 2,
      key: 'base64Y3YxN2E1MWFlYw=='
    }
  ],
  deviceId: '4c299165-6e8f-4b45-a5ba-c5d250a707ff',
  displayName: 'Test device',
  operatingSystem: 'linux',
  operatingSystemVersion: '1'
};

await client.api('/devices')
    .post(device);

```