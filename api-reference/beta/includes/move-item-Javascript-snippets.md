---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 6cfa6c5e1b51d8b280036455a958f2e4025e1034
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34443843"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const driveItem = {
  parentReference: {
    id: "new-parent-folder-id"
  },
  name: "new-item-name.txt"
};

let res = await client.api('/me/drive/items/{item-id}')
    .version('beta')
    .update({driveItem : driveItem});

```