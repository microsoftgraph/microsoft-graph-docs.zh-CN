---
description: 自动生成的文件。 不修改
ms.openlocfilehash: ea487b7587515bffa9662b4cdad27cee28fb8078
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35478595"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const workbookSessionInfo = {
  persistChanges: true
};

let res = await client.api('/me/drive/items/{id}/workbook/createSession')
    .version('beta')
    .post(workbookSessionInfo);

```