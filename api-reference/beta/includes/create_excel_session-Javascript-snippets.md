---
description: 自动生成的文件。 不修改
ms.openlocfilehash: ea487b7587515bffa9662b4cdad27cee28fb8078
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34480748"
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