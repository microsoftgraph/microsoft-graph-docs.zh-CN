---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 20941e363965e9fdaa08b6672fcfa7d30cd7f61a
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50788077"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const message = {
    message: {
      attachments: [ 
        { 
          '@odata.type': '#microsoft.graph.fileAttachment', 
          name: 'guidelines.txt', 
          contentBytes: 'bWFjIGFuZCBjaGVlc2UgdG9kYXk=' 
        } 
      ]
    },
    comment: 'if the project gets approved, please take a look at the attached guidelines before you decide on the name.' 
};

await client.api('/me/messages/AAMkADA1MTAAAH5JaKAAA=/createReplyAll')
    .version('beta')
    .post(message);

```