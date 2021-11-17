---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ebf2639d0c9e02974d1d30df47059cf9bf25c144d50648c5db42086e21854f82
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57277337"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const tentativelyAccept = {
  comment: 'I may not be able to make this week. How about next week?',
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

await client.api('/me/events/{id}/tentativelyAccept')
    .version('beta')
    .post(tentativelyAccept);

```