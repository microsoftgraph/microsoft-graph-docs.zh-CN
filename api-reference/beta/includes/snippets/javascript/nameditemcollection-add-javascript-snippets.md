---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e6009200e302751ff81d7e65e31d869184debc76
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50785632"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const workbookNamedItem = {
  name: 'test7',
  formula: '=SUM(Sheet2!$A$1+Sheet2!$A$2)',
  comment: 'Comment for the named item'
};

await client.api('/me/drive/items/{id}/workbook/names/addFormulaLocal')
    .version('beta')
    .post(workbookNamedItem);

```