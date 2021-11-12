---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 08ce01b915b235aaa78a05ca7289db1d22c3658324ab0ba08dfc563b96002f7f
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57105474"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const workbookTable = {
  address: 'A1:D8',
  hasHeaders: false
};

await client.api('/me/drive/items/{id}/workbook/tables/$/add')
    .version('beta')
    .post(workbookTable);

```