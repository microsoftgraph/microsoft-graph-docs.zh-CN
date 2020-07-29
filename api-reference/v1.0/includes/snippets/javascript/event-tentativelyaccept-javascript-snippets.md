---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d7094a8cbcab23f72b4202b9a136e6bec249b591
ms.sourcegitcommit: 9faca60f0cc4ee9d6dce33fd25c72e14b5487d34
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/29/2020
ms.locfileid: "46512212"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const tentativelyAccept = {
  comment: "I may not be able to make this week. How about next week?",
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

let res = await client.api('/me/events/{id}/tentativelyAccept')
    .post(tentativelyAccept);

```