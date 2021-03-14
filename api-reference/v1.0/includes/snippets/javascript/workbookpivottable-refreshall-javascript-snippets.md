---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ffa73b4b9dccbbdaf88ce08cb52b87be0505850e
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50807754"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/me/drive/root/workbook/worksheets/{id}/pivotTables/refreshAll')
    .post();

```