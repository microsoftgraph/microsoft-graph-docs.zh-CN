---
description: 自动生成的文件。 不修改
ms.openlocfilehash: e328f7d44310f20f7a2228df25589dd6ff05fd12
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35713431"
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
    .post({device : device});

```