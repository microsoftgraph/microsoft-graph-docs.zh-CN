---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 37a2658d9c4dcb30632ed49d2ac10cc5fd3afbd1
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34462237"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/teams/{teamId}/schedule')
    .version('beta')
    .get();

```