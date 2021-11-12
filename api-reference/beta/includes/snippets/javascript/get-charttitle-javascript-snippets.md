---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 664b80920330f8208de98bfe98a345e4b9ce29ba6dc55112a44a3e2064627df1
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57220339"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let workbookChartTitle = await client.api('/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/title')
    .version('beta')
    .get();

```