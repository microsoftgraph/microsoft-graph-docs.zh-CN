---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 44b9fd8abe4fb76313ea7cd1aa54c6dca373ffe3
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34435373"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/drive/items/{id}/workbook/tables/{id|name}/sort/reapply')
    .post();

```