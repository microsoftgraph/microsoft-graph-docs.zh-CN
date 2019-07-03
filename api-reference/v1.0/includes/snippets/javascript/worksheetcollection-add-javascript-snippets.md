---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 94fa1baa5887f9d4cb5a4665c567deb4bf7908c5
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35493370"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const workbookWorksheet = {
  name: "name-value"
};

let res = await client.api('/me/drive/items/{id}/workbook/worksheets/add')
    .post(workbookWorksheet);

```