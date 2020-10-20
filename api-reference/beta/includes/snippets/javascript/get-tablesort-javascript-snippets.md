---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0772aa2e4c1b7f218654082f6aec1c3cd35e39a8
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/20/2020
ms.locfileid: "48614185"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/drive/items/{id}/workbook/tables/{id|name}/sort')
    .version('beta')
    .get();

```