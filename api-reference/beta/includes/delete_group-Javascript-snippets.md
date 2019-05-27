---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 2bd88383bf2578903972219354f636a6d6a420ce
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34438299"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/groups/{id}')
    .version('beta')
    .delete();

```