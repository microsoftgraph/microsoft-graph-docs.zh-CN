---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 99887cccfe14825608ae39738ce160968c6bdf68c55eab3d9a58e5a638de60d2
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57279370"
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
         id: '8c0a1a67-50ce-4114-bb6c-da9c5dbcf6ca',
         displayName: 'John Doe'
      }
   },
   body: {
      contentType: 'html',
      content: 'Hello World'
   }
};

await client.api('/teams/57fb72d0-d811-46f4-8947-305e6072eaa5/channels/19:4b6bed8d24574f6a9e436813cb2617d8@thread.tacv2/messages/1590776551682/replies')
    .post(chatMessage);

```