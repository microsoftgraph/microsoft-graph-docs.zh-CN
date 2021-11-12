---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d1689687a3c5681d198c2be1d29a350ed00e13cffa56a804f8012f3a9c6f394c
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57106583"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const workbookWorksheet = {
  name: 'name-value'
};

await client.api('/me/drive/items/{id}/workbook/worksheets/add')
    .version('beta')
    .post(workbookWorksheet);

```