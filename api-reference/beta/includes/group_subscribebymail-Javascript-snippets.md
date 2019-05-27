---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 36bb2d3d2a8b2317fc41f1fae6a1c4b53b6289c2
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34444690"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/groups/{id}/subscribeByMail')
    .version('beta')
    .post();

```