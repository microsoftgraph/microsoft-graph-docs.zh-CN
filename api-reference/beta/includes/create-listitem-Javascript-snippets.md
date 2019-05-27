---
description: 自动生成的文件。 不修改
ms.openlocfilehash: a8fb6a95928980c79cd2b7a0c7f4333075484738
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34460746"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const fieldValueSet = {
    Color: "Fuchsia",
    Quantity: 934
};

let res = await client.api('/sites/{site-id}/lists/{list-id}/items/{item-id}/fields')
    .version('beta')
    .update({fieldValueSet : fieldValueSet});

```