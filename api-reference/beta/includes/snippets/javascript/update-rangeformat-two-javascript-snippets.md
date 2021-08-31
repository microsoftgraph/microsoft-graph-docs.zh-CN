---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e5bb386de52a33abc510e049192ccff54d8ab57b1daca1094e192b70bf7d6b2d
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57162465"
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

await client.api('/me/drive/items/{id}/workbook/worksheets/Sheet1/range(address='$B$1')/format')
    .version('beta')
    .update(workbookRangeFormat);

```