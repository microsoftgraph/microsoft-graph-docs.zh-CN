---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 210e402cfc4b97a03e44ec48e99a7ea4c787d224
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34481070"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const directorySetting = {
  directorySetting: {
    displayName: "displayName-value",
    templateId: "templateId-value",
    values: [
      {
        name: "name-value",
        value: "value-value"
      }
    ]
  }
};

let res = await client.api('/groups/{id}/settings')
    .version('beta')
    .post({directorySetting : directorySetting});

```