---
description: 自动生成的文件。 不修改
ms.openlocfilehash: ce675f51249ab638a885ad83aef1fec763c5b713
ms.sourcegitcommit: 3db93e28e215c0e09a65b4705ba956c6ac3b5426
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/14/2019
ms.locfileid: "36396875"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const user = {
  businessPhones: [
    "businessPhones-value"
  ],
  officeLocation: "city-value"
};

let res = await client.api('/me')
    .version('beta')
    .update({user : user});

```