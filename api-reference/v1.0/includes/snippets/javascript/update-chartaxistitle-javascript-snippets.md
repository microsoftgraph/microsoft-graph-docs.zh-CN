---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 86da403a3bf35b14ac26125c41735b46ef91ed6f
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50805801"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const workbookChartAxisTitle = {
  text: 'text-value',
  visible: true
};

await client.api('/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/axes/valueAxis/title')
    .update(workbookChartAxisTitle);

```