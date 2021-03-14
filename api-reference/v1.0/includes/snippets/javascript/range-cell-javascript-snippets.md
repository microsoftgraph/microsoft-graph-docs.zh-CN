---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 518140c745d99c66f3622375e2390ddcc17bfde5
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50790719"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let workbookRange = await client.api('/me/drive/items/{id}/workbook/names/{name}/range/cell(row=5,column=6)')
    .get();

```