---
description: 自动生成的文件。 不修改
ms.openlocfilehash: bab95dbfa2f2c8b34ac3bb67734ce3858bdbddfe
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34444081"
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