---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8e2cce82534095029360be346597a74132dedc81
ms.sourcegitcommit: 7e1993d64cc6d3145ae0ca984fefe74772b6052b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/16/2020
ms.locfileid: "47938434"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const externalItem = {
  acl: [
    {
      type: "user",
      value: "49103559-feac-4575-8b94-254814dfca72",
      accessType: "grant",
      identitySource: "azureActiveDirectory"
    }
  ]
};

let res = await client.api('/connections/contosohr/items/TSP228082938')
    .version('beta')
    .update(externalItem);

```