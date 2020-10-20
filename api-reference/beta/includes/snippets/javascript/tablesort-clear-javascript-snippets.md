---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f3b2e367d59c87eccd9cc1c22aa8c2597a99b562
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/20/2020
ms.locfileid: "48617605"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/drive/items/{id}/workbook/tables/{id|name}/sort/clear')
    .version('beta')
    .post();

```