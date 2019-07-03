---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 3ac52e8439bddb9d5020d35300fccfaa43101738
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35493101"
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
    .post(workbookSessionInfo);

```