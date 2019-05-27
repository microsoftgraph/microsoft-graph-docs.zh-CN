---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 191ec0b1d2a6103c3b3b1e6708fcb1f6d19d5721
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34471513"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/groups/{id}/endpoints/{id}')
    .version('beta')
    .get();

```