---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a4ec9c3e1688821aa5de484e7c53af91c7ae7dff
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50794193"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const setData = {
  sourceData: 'sourceData-value',
  seriesBy: 'seriesBy-value'
};

await client.api('/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/setData')
    .post(setData);

```