---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ce315ea7a1c5453ada11450478ae079e3ca651f7
ms.sourcegitcommit: c9b9ff2c862f8d96d282a7bdf641cdb9c53a4600
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2019
ms.locfileid: "37636943"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const decline = {
  comment: "I won't be able to make this week. How about next week?",
  sendResponse: true,
  proposedNewTime: {
      start: { 
          dateTime: "2019-12-02T18:00:00", 
          timeZone: "Pacific Standard Time" 
      }, 
      end: { 
          dateTime: "2019-12-02T19:00:00", 
          timeZone: "Pacific Standard Time" 
      }     
  }
};

let res = await client.api('/me/events/{id}/decline')
    .version('beta')
    .post(decline);

```