---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: eb89df6a2b08a866dc3caf98bff1d873022a2562
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50799728"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let workbookTableSort = await client.api('/me/drive/items/{id}/workbook/tables/{id|name}/sort')
    .version('beta')
    .get();

```