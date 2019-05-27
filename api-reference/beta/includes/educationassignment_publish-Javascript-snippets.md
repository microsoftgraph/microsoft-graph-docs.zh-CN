---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 161636dac4a8270b9693d1594bf25b3a9ba6b08a
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34436969"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/education/classes/11021/assignments/19002/publish')
    .version('beta')
    .post();

```