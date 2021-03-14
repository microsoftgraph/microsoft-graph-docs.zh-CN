---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ae0d2732ecd33317a3b912fc78b595a3de552d6b
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50790888"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let workbookWorksheet = await client.api('/me/drive/items/{id}/workbook/worksheets/{id|name}')
    .get();

```