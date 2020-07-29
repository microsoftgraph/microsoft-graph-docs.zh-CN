---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 90f6198e95ee83fbf9a8bbf67736e9855a87a06d
ms.sourcegitcommit: 9faca60f0cc4ee9d6dce33fd25c72e14b5487d34
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/29/2020
ms.locfileid: "46512278"
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
    .post(decline);

```