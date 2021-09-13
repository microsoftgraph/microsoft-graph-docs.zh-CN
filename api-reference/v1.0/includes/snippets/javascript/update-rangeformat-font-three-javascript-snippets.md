---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b9eade7a6c7aba9d5fd366924df91fac95574d8db1cc36f0f0522c595b88f4de
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57105377"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const workbookRangeFont = {
  underline: 'Single',
  color: '#FFFFFF',
  size: 26
};

await client.api('/me/drive/items/{id}/workbook/worksheets/{sheet-id}/range(address='$C$1')/format/font')
    .update(workbookRangeFont);

```