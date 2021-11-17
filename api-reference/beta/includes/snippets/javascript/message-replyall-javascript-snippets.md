---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6f7bc1314b764001c561dc8c43c8c29c4d0329c53e6f79085cbd8e0fc2207e35
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57104382"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const replyAll = {
    message: {
      attachments: [ 
        { 
          '@odata.type': '#microsoft.graph.fileAttachment', 
          name: 'guidelines.txt', 
          contentBytes: 'bWFjIGFuZCBjaGVlc2UgdG9kYXk=' 
        } 
      ]
    },
    comment: 'Please take a look at the attached guidelines before you decide on the name.' 
};

await client.api('/me/messages/AAMkADA1MTAAAH5JaKAAA=/replyAll')
    .version('beta')
    .post(replyAll);

```