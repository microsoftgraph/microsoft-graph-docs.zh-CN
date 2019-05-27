---
description: 自动生成的文件。 不修改
ms.openlocfilehash: de4951d8c8ef3a2db535146aefbaea2cbda803b5
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34448976"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/contacts/{id}/memberOf')
    .version('beta')
    .get();

```