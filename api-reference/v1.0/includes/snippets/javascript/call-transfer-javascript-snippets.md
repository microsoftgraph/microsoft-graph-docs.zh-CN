---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5c63165ea02724a28a5b66b3a22b288914b3260d
ms.sourcegitcommit: 42fdb068616222eb6b0813e93b33e830fc7eedc0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/17/2021
ms.locfileid: "50274771"
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
        phone: {
          @odata.type: "#microsoft.graph.identity",
          id: "+12345678901"
        }
    },
    languageId: "languageId-value",
    region: "region-value"
  },
  clientContext: "9e90d1c1-f61e-43e7-9f75-d420159aae08"
};

let res = await client.api('/communications/calls/{id}/transfer')
    .post(transfer);

```