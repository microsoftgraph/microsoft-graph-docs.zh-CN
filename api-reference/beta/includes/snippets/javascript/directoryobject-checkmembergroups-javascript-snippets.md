---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 5b857056c27f35eb3eeea13f56706a47d37dd16c
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35520946"
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