---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 67c89aaf68e7dcda76e5f30837b3913808004c9d
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34454129"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const _delete = {
  shift: "shift-value"
};

let res = await client.api('/me/drive/items/{id}/workbook/names/{name}/range/delete')
    .post(_delete);

```