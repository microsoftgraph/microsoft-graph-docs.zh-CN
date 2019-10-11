---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e00bec9374b6ca56e939b3b0ce3929947cc400ad
ms.sourcegitcommit: 1585d55d3e7030b5fd1f7cfd5de8f9fb8202cd56
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/09/2019
ms.locfileid: "37428802"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const string = {
  groupIds: [
        "fee2c45b-915a-4a64-b130-f4eb9e75525e",
        "4fe90ae7-065a-478b-9400-e0a0e1cbd540"
  ]
};

let res = await client.api('/me/checkMemberGroups')
    .version('beta')
    .post(string);

```