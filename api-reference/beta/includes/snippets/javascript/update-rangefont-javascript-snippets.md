---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 44ec59c9d4dd8e5890e9b7a59e9d64af6cbd225f32383f545b9d213e8e8d6d2f
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57332479"
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