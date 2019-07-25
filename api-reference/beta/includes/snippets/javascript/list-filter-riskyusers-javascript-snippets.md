---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 64df205982730e669bb75ab9f5ec5cad389477fe
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35718271"
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