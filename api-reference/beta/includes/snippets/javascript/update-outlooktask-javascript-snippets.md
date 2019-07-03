---
description: 自动生成的文件。 不修改
ms.openlocfilehash: b0fe630be99028d4983e0fc0f2ea9a11d24f426b
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35520117"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const outlookTask = {
  dueDateTime:  {
      dateTime: "2016-05-06T16:00:00",
      timeZone: "Eastern Standard Time"
  }
};

let res = await client.api('/me/outlook/tasks/AAMkADA1MTHgwAAA=')
    .version('beta')
    .update({outlookTask : outlookTask});

```