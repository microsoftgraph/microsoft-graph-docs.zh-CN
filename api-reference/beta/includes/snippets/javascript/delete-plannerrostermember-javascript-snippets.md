---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1fdbe2d3ff6830c8ab36cdc3d362667c609808d7
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50781330"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/planner/rosters/523a9d5a-f9d5-45c1-929f-b8525393515c/members/5ba84f7a-aa11-4a51-a298-9f2c7ec6bb38')
    .version('beta')
    .delete();

```