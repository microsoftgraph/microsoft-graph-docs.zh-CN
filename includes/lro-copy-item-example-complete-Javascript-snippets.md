---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 466b3df441f1ef0b468512e6ed894ec765b86cd2
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34843694"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/drive/items/{item-id}')
    .version('beta')
    .get();

```