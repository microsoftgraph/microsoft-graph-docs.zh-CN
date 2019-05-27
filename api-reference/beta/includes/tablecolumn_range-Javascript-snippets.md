---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 2a5360aa2e5a89724e917852baee3225cc24b6f7
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34482442"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/drive/items/{id}/workbook/tables/{id|name}/columns/{id|name}/Range')
    .version('beta')
    .post();

```