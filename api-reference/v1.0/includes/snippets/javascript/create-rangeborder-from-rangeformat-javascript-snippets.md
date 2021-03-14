---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 157677622b04ee44541dce1bf6966974ef235a5c
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50785527"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const workbookRangeBorder = {
  id: 'id-value',
  color: 'color-value',
  style: 'style-value',
  sideIndex: 'sideIndex-value',
  weight: 'weight-value'
};

await client.api('/me/drive/items/{id}/workbook/names/{name}/range/format/borders')
    .post(workbookRangeBorder);

```