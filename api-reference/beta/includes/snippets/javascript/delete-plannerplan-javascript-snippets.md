---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 2c54087fa94f63afd111f5cad6aa3da4388cac3b
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/15/2019
ms.locfileid: "36413344"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/planner/plans/{id}')
    .version('beta')
    .delete();

```