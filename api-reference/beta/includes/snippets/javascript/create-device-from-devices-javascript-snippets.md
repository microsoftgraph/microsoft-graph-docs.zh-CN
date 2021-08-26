---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c2c7e222744e668d07d8ec5ae34a6f7a8a620c871f806d1e4492f9ebfa46a199
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57218594"
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
      identityProvider: 'identityProvider-value',
      key: 'base64Y3YxN2E1MWFlYw=='
    }
  ],
  approximateLastSignInDateTime: '2016-10-19T10:37:00Z',
  deviceId: 'deviceId-value',
  deviceMetadata: 'deviceMetadata-value',
  deviceVersion: 99
};

await client.api('/devices')
    .version('beta')
    .post(device);

```