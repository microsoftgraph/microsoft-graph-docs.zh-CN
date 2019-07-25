---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 1c9bc81f713a268d73888a3b86927986bb811650
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35722600"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const event = {
  location:{
      displayName:"Conf Room 2"
  }
};

let res = await client.api('/groups/01d4ee64-15ce-491e-bad1-b91aa3223df4/calendar/events/AAMkADZlAAAAABERAAA=')
    .update({event : event});

```