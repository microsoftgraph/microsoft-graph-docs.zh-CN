---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3675f5cebe33781936987e94db97f2c0836268ac
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50804617"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const reply = {
  post: {
    body: {
      contentType: 'text',
      content: 'Which quarter does that file cover? See my attachment.'
    },
    attachments: [{
      '@odata.type': '#microsoft.graph.fileAttachment',
      name: 'Another file as attachment',
      contentBytes: 'VGhpcyBpcyBhIGZpbGUgdG8gYmUgYXR0YWNoZWQu'
    } ]
  }
};

await client.api('/groups/1848753d-185d-4c08-a4e4-6ee40521d115/threads/AAQkADJUdfolA==/reply')
    .version('beta')
    .post(reply);

```