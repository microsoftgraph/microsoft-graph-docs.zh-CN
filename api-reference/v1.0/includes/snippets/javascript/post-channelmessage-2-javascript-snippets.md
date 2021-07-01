---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4f3e6ba16dfe7d37b47dab67f8eb61333fee57cd
ms.sourcegitcommit: fe1b4d098af604cc34596f595e799911ea672532
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/07/2021
ms.locfileid: "51611577"
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