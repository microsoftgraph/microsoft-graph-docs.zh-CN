---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 31cb3a18476c1b94d82e234bf7c6c0e517350c85
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34471429"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/messages/AAMkADYAAAImV_jAAA=/')
    .version('beta')
    .expand('eventMessage/event')
    .get();

```