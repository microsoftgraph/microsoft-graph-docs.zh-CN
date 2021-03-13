---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 86b0fe6c2f1a5f4fed0ad0f8858489542464784e
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50808959"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const workbookRangeFont = {
  bold: true,
  color: 'color-value',
  italic: true,
  name: 'name-value',
  size: 99,
  underline: 'underline-value'
};

await client.api('/me/drive/items/{id}/workbook/names/{name}/range/format/font')
    .version('beta')
    .update(workbookRangeFont);

```