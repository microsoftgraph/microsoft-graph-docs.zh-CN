---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 5b857056c27f35eb3eeea13f56706a47d37dd16c
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34437228"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const String = {
  groupIds: [
        "fee2c45b-915a-4a64-b130-f4eb9e75525e",
        "4fe90ae7-065a-478b-9400-e0a0e1cbd540"
  ]
};

let res = await client.api('/me/checkMemberGroups')
    .version('beta')
    .post(String);

```