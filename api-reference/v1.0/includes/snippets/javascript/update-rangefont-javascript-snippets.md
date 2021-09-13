---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ea9913092007fc0fd42835bf687ef79a3e9fe5745782bc20f3e67213272893f5
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57162949"
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
    .update(workbookRangeFont);

```