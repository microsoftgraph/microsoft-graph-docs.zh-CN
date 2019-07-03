---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 35c23382325e1ff96a1735d7f30e80ce58bb5c1e
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35519556"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const replyAll = {
    message:{
      attachments: [ 
        { 
          @odata.type: "#microsoft.graph.fileAttachment", 
          name: "guidelines.txt", 
          contentBytes: "bWFjIGFuZCBjaGVlc2UgdG9kYXk=" 
        } 
      ]
    },
    comment: "Please take a look at the attached guidelines before you decide on the name." 
};

let res = await client.api('/me/messages/AAMkADA1MTAAAH5JaKAAA=/replyAll')
    .version('beta')
    .post(replyAll);

```