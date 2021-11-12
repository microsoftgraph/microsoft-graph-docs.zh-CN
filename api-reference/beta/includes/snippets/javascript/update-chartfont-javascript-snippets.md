---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d715fb2eb7824f1f579a8509743a13bbf965a297bd543193f0a4ddb0cfe778f3
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57219272"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const workbookChartFont = {
  bold: true,
  color: 'color-value',
  italic: true,
  name: 'name-value',
  size: 99,
  underline: 'underline-value'
};

await client.api('/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/axes/valueaxis/format/font')
    .version('beta')
    .update(workbookChartFont);

```