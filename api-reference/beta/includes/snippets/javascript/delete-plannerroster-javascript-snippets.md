---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a1f84be0ea9c7e0a879eb7137ecaedbfaa8e16a1
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50803279"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/planner/rosters/5ba84f7a-aa11-4a51-a298-9f2c7ec6bb38')
    .version('beta')
    .delete();

```