---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c96552d70740f00887d11077cf7317429d89499bc9569768d105ba2b3503ecf9
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57104279"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let workbookRange = await client.api('/me/drive/items/{id}/workbook/tables/{id|name}/columns/{id|name}/headerRowRange')
    .get();

```