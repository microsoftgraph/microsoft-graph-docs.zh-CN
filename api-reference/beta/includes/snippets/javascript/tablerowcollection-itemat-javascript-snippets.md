---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4462fa419730ec536713f34a431a2d2874dc98023d83f93f220a29091c132712
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57162718"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const workbookTableRow = {
  index: {
  }
};

await client.api('/me/drive/items/{id}/workbook/tables/{id|name}/rows/ItemAt')
    .version('beta')
    .post(workbookTableRow);

```