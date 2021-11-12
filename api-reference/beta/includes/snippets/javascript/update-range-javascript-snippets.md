---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d23970028be89af44c9ca74372ff6947201e484e08ed461bbe05350522766342
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57220245"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const workbookRange = {
values: [['Hello', '100'],['1/1/2016', null]],
formulas: [[null, null], [null, '=B1*2']],
numberFormat: [[null,null], ['m-ddd', null]]
};

await client.api('/me/drive/items/{id}/workbook/worksheets/sheet1/range(address='A1:B2')')
    .version('beta')
    .update(workbookRange);

```