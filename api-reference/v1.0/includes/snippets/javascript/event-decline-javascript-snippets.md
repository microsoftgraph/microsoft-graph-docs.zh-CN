---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 23eaf8062bf3bb9df0c956ab5999e0f820717c1b71afc46dd59430864999df9a
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57218789"
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