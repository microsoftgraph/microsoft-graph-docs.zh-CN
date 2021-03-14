---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 930bc5b6385e103f1e7fa4e572a946164cba2ca4
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50782904"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let workbookNamedItem = await client.api('/me/drive/items/{id}/workbook/names/{name}')
    .get();

```