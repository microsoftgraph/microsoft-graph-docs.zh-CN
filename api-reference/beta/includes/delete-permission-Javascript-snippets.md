---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 3a22207a0c999cab19d39407649cc12fa23f2a9a
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34439181"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/drive/root/items/{item-id}/permissions/{perm-id}')
    .version('beta')
    .delete();

```