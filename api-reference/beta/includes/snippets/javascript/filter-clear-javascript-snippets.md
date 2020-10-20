---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1cedeed37f957d830bebd206b4652e2019eb7b54
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/20/2020
ms.locfileid: "48613364"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/drive/items/{id}/workbook/tables/{id|name}/columns/{id|name}/filter/clear')
    .version('beta')
    .post();

```