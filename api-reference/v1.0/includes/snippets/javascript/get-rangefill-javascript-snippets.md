---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7622da35107b7703dcfaa3bd2b82776e4c4422db
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50809574"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let workbookRangeFill = await client.api('/me/drive/items/{id}/workbook/names/{name}/range/format/fill')
    .get();

```