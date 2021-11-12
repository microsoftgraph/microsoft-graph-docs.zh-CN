---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 116f97a2b4e48d2be93b574aa454f43e7964c81d481397a3edcce98ccb4b4f90
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57163880"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const workbookTable = {
  address: '',
  hasHeaders: false
};

await client.api('/me/drive/items/{id}/workbook/worksheets/{id|name}/tables/$/add')
    .version('beta')
    .post(workbookTable);

```