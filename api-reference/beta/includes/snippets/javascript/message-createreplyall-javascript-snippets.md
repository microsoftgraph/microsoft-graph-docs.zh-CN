---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b60534b529be4c353c69f8b6ff517ae4f4cf04a55bfc37db931703c31894efc2
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57220641"
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