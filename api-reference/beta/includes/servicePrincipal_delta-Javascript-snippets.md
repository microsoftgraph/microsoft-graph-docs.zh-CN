---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 7db48d9ce03407aa90d82f0256322371c2e7c019
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34469467"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/servicePrincipals/delta')
    .version('beta')
    .get();

```