---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 26f462438b3f5a50c47472c80c243c668c1f9c46
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/20/2020
ms.locfileid: "48610059"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/drive/items/{id}/workbook/worksheets/{id|name}/UsedRange(valuesOnly=true)')
    .version('beta')
    .get();

```