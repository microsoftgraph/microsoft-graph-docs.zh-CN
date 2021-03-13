---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2ead259d69343162a03c16a5109c9c77b97d88ed
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50778831"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const workbookSessionInfo = {
  persistChanges: true
};

await client.api('/me/drive/items/{id}/workbook/createSession')
    .version('beta')
    .post(workbookSessionInfo);

```