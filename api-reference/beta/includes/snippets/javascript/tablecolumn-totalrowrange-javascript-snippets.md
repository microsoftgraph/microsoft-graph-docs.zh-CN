---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 76d1e576fecbeecbc26d7e96c60311497dd35528
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/20/2020
ms.locfileid: "48621185"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/drive/items/{id}/workbook/tables/{id|name}/columns/{id|name}/TotalRowRange')
    .version('beta')
    .post();

```