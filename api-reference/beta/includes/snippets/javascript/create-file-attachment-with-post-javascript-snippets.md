---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 852ae44b258da8707aaa3afd211d430372195ec5
ms.sourcegitcommit: 0329bbcd5f1b09a2a6c5f935a30c4560b6eed492
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/27/2019
ms.locfileid: "36633557"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const reply = {
  post: {
    body: {
      contentType: "text",
      content: "Which quarter does that file cover? See my attachment."
    },
    attachments: [{
      @odata.type: "#microsoft.graph.fileAttachment",
      name: "Another file as attachment",
      contentBytes: "VGhpcyBpcyBhIGZpbGUgdG8gYmUgYXR0YWNoZWQu"
    } ]
  }
};

let res = await client.api('/groups/1848753d-185d-4c08-a4e4-6ee40521d115/threads/AAQkADJUdfolA==/reply')
    .version('beta')
    .post(reply);

```