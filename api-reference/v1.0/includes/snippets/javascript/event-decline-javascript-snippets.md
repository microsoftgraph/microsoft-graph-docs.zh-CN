---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b39ddbd12da6e60f5c0b1b5f49c175adb74fc646
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50780853"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const decline = {
  comment: 'I won\'t be able to make this week. How about next week?',
  sendResponse: true,
  proposedNewTime: {
      start: { 
          dateTime: '2019-12-02T18:00:00', 
          timeZone: 'Pacific Standard Time' 
      }, 
      end: { 
          dateTime: '2019-12-02T19:00:00', 
          timeZone: 'Pacific Standard Time' 
      }     
  }
};

await client.api('/me/events/{id}/decline')
    .post(decline);

```