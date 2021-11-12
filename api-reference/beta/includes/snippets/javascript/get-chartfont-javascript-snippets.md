---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 75548121e7873bd556afbdd57a3e502863c8445b65435cf19bd9fba3a34e1ea6
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57278430"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let workbookChartFont = await client.api('/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/axes/valueaxis/format/font')
    .version('beta')
    .get();

```