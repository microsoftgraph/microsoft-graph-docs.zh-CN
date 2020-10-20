---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e362800b9ff4d854d7a4e726097ba180ede1654b
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/20/2020
ms.locfileid: "48608883"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/drive/items/{id}/workbook/tables/{id|name}/clearFilters')
    .version('beta')
    .post();

```