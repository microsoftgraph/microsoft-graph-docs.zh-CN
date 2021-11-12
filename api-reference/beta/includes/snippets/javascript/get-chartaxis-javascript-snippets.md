---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 16b237f193cabfcb28c5430981aaaffcc69bf68496caa927848c8f9a6c0ff317
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56903116"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let workbookChartAxis = await client.api('/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/axes/valueaxis')
    .version('beta')
    .get();

```