---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: afe2f484698d7420b1ef1928eabf7f19ea2f48c30a28d97679ed5474c9b97f5d
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57105378"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const workbookRangeFormat = {
  columnWidth: 135,
  horizontalAlignment: 'Center',
  verticalAlignment: 'Center',
  rowHeight: 49,
  wrapText: false
};

await client.api('/me/drive/items/{id}/workbook/worksheets/{sheet-id}/range(address='$B$1')/format')
    .update(workbookRangeFormat);

```