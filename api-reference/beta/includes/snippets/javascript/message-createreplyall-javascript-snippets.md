---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: bab95dbfa2f2c8b34ac3bb67734ce3858bdbddfe
ms.sourcegitcommit: d4114bac58628527611e83e436132c6581a19c52
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/13/2020
ms.locfileid: "35729666"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const message = {
    message:{
      attachments: [ 
        { 
          @odata.type: "#microsoft.graph.fileAttachment", 
          name: "guidelines.txt", 
          contentBytes: "bWFjIGFuZCBjaGVlc2UgdG9kYXk=" 
        } 
      ]
    },
    comment: "if the project gets approved, please take a look at the attached guidelines before you decide on the name." 
};

let res = await client.api('/me/messages/AAMkADA1MTAAAH5JaKAAA=/createReplyAll')
    .version('beta')
    .post(message);

```