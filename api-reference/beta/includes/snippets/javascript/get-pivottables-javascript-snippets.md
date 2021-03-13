---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: eb4fe1881e88766055612c7828bcb2af7ca9e5f9
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50793960"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let pivotTables = await client.api('/drive/root/workbook/worksheets/{id}/pivotTables')
    .version('beta')
    .get();

```