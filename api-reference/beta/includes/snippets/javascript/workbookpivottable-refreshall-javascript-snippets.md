---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8a1cc347cf1ef4bb382f1e1e80ea91dadca81938
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50782242"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/drive/root/workbook/worksheets/{id}/pivotTables/refreshAll')
    .version('beta')
    .post();

```