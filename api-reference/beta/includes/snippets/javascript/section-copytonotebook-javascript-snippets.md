---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 361f71b146a319a6639ffd9498435f407178496d
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35725519"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const onenoteOperation = {
  id: "id-value",
  groupId: "groupId-value",
  renameAs: "renameAs-value"
};

let res = await client.api('/me/onenote/sections/{id}/copyToNotebook')
    .version('beta')
    .post(onenoteOperation);

```