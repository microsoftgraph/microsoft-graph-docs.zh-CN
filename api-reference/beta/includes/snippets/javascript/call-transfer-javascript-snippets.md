---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 11fc657409b34dec6d4b3e8e7a341270729c3a72
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35708798"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const transfer = {
  transferTarget: {
    endpointType: "default",
    identity: {
      user: {
        id: "550fae72-d251-43ec-868c-373732c2704f",
        tenantId: "72f988bf-86f1-41af-91ab-2d7cd011db47",
        displayName: "Heidi Steen"
      }
    },
    languageId: "languageId-value",
    region: "region-value",
    replacesCallId: "replacesCallId-value"
  },
  clientContext: "clientContext-value"
};

let res = await client.api('/app/calls/{id}/transfer')
    .version('beta')
    .post(transfer);

```