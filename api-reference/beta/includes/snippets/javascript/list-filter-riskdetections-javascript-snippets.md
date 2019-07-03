---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 1112dce24b0f15761d91316acdd3bdc742bd40a7
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35478936"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/riskDetections')
    .version('beta')
    .filter('riskType eq 'unfamiliarFeatures' or riskLevel eq 'medium'')
    .get();

```