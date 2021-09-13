---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 60a2462784a4e3135240be10f51ad48832f7420bd41040858f9d93c58601faf2
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57164218"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let workbookRange = await client.api('/me/drive/root/workbook/worksheets/{id}/range/rowsBelow(count=2)')
    .get();

```