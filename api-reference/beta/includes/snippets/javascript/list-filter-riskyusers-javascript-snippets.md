---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 64df205982730e669bb75ab9f5ec5cad389477fe
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35478938"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/riskyUsers')
    .version('beta')
    .filter('riskLevel eq microsoft.graph.riskLevel'medium'')
    .get();

```