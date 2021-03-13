---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 89a00b73cf5454db0aefbf0e31c4107ffac631de
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50783134"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const workbookTable = {
  address: 'Sheet1!A1:D5',
  hasHeaders: true
};

await client.api('/me/drive/items/{id}/workbook/tables/add')
    .version('beta')
    .post(workbookTable);

```