---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 6e9244f62bf7857aa08c8b53a68bb8d736ef588a
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34436822"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/drive/items/{item-id}/thumbnails')
    .version('beta')
    .get();

```