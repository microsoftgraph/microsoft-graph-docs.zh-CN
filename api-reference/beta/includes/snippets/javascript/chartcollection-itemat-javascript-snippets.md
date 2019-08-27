---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 00aa9455cf63ac4c6e7fbcfc95b7edba7c032816
ms.sourcegitcommit: 0329bbcd5f1b09a2a6c5f935a30c4560b6eed492
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/27/2019
ms.locfileid: "36636560"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const workbookChart = {
  index: 8
};

let res = await client.api('/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/ItemAt')
    .version('beta')
    .post(workbookChart);

```