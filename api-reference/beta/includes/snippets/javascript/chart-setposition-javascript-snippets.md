---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e986188c8d03f12f269935df5a70786d8cb0ff9c
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50801050"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const setPosition = {
  startCell: 'startCell-value',
  endCell: 'endCell-value'
};

await client.api('/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/setPosition')
    .version('beta')
    .post(setPosition);

```