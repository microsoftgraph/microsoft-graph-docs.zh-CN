---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 04a45659c47f1f5457f6a5d2b3bd22921acaf6b6
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34459677"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/drive/items/{item-id}/permissions/{perm-id}')
    .delete();

```