---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ffb8891083dd534422e890c72b829ff296094d6a8057d20725044f198ea5d8d6
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57274339"
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