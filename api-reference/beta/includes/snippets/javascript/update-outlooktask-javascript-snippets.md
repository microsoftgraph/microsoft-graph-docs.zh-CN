---
description: 自动生成的文件。 不修改
ms.openlocfilehash: d6179e2f010b3adac07cdf83654768a192926ed3
ms.sourcegitcommit: 0329bbcd5f1b09a2a6c5f935a30c4560b6eed492
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/27/2019
ms.locfileid: "36636664"
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
    .update(outlookTask);

```