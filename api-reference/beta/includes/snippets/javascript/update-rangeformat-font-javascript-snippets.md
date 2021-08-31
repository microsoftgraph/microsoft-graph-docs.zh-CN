---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a7da9a16723c633be6977219f2c33fc106c6e62c6b3ccfd507cf5fd07c4430fc
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57106307"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const workbookRangeFont = {
  bold: true,
  color: '#4B180E',
  size: 26
};

await client.api('/me/drive/items/{id}/workbook/worksheets/Sheet1/range(address='$A$1')/format/font')
    .version('beta')
    .update(workbookRangeFont);

```