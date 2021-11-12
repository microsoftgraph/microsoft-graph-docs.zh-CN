---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8f6a87d356aef45b4296aa3aef3f10b0a99afc442c358f1b67fb887e1be1555e
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57104893"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let workbookChartAxisTitle = await client.api('/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/axes/valueaxis/title')
    .version('beta')
    .get();

```