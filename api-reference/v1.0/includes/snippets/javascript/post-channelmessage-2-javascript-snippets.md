---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8f252d000498431e1dd0210bc2656dafaa84356be408bcea448cf6c8c7b0ef0c
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57409778"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const chatMessage = {
   createdDateTime: '2019-02-04T19:58:15.511Z',
   from: {
      user: {
         id: 'id-value',
         displayName: 'Joh Doe',
         userIdentityType: 'aadUser'
      }
   },
   body: {
      contentType: 'html',
      content: 'Hello World'
   }
};

await client.api('/teams/57fb72d0-d811-46f4-8947-305e6072eaa5/channels/19:4b6bed8d24574f6a9e436813cb2617d8@thread.tacv2/messages')
    .post(chatMessage);

```