---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 73c57c7fee03b2cc1fa0e9f3836df25e2891ef7b
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/20/2020
ms.locfileid: "48616468"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/title')
    .version('beta')
    .get();

```