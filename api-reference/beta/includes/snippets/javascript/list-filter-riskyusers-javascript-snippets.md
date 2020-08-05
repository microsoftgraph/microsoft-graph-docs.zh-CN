---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c7b6f38f25300135e0ccc8f5ac1475efeb36f5fb
ms.sourcegitcommit: 496410c1e256aa093eabf27f17e820d9ee91a293
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2020
ms.locfileid: "46570139"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/identityProtection/riskyUsers')
    .version('beta')
    .filter('riskLevel eq microsoft.graph.riskLevel'medium'')
    .get();

```