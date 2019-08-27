---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 80258ba927597036d7fcdcf3519a3f1ceac91662
ms.sourcegitcommit: 0329bbcd5f1b09a2a6c5f935a30c4560b6eed492
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/27/2019
ms.locfileid: "36636541"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const device = {
  accountEnabled: true,
  alternativeSecurityIds: [
    {
      type: 99,
      identityProvider: "identityProvider-value",
      key: "base64Y3YxN2E1MWFlYw=="
    }
  ],
  approximateLastSignInDateTime: "2016-10-19T10:37:00Z",
  deviceId: "deviceId-value",
  deviceMetadata: "deviceMetadata-value",
  deviceVersion: 99
};

let res = await client.api('/devices')
    .version('beta')
    .post(device);

```