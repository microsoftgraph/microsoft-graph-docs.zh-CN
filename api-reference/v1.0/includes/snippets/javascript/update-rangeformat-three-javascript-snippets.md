---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c6e1d406112c97e36b021cc86339dfa52d4728c44e7950ae4ee3747b059df09b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57161801"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const workbookRangeFormat = {
  columnWidth: 135,
  horizontalAlignment: 'Right',
  verticalAlignment: 'Top',
  rowHeight: 49,
  wrapText: false
};

await client.api('/me/drive/items/{id}/workbook/worksheets/{sheet-id}/range(address='$C$1')/format')
    .update(workbookRangeFormat);

```