---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f6dd877cacf2aefc7209ec5eb603c0d8c51c64c1
ms.sourcegitcommit: 0329bbcd5f1b09a2a6c5f935a30c4560b6eed492
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/27/2019
ms.locfileid: "36636839"
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
    .update(event);

```