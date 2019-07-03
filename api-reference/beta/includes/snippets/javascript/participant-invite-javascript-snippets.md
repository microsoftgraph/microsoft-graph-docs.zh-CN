---
description: 自动生成的文件。 不修改
ms.openlocfilehash: e0188059c57aa7cccca7ca0801ff86379fadadf5
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35521075"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const CommsOperation = {
  participants: [
    {
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
    }
  ],
  clientContext: "clientContext-value"
};

let res = await client.api('/app/calls/{id}/participants/invite')
    .version('beta')
    .post(CommsOperation);

```