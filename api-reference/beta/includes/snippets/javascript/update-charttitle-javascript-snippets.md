---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 54f180b632477d2ab10d8a3296e9ce4132e02a9c
ms.sourcegitcommit: 0329bbcd5f1b09a2a6c5f935a30c4560b6eed492
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/27/2019
ms.locfileid: "36636550"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const workbookChartTitle = {
  overlay: true,
  text: "text-value",
  visible: true
};

let res = await client.api('/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/title')
    .version('beta')
    .update(workbookChartTitle);

```