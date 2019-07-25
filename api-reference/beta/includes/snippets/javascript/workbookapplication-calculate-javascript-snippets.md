---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 24e3db47dbc7b9480e86c282070f25dc6c70660c
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35723755"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const calculate = {
  calculationType: "calculationType-value"
};

let res = await client.api('/me/drive/items/{id}/workbook/application/calculate')
    .version('beta')
    .post(calculate);

```