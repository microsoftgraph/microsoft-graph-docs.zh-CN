---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 81c0e73ecacba11858168cb345fc22d519726488
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34449557"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/groupLifecyclePolicies')
    .version('beta')
    .get();

```