---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 7f546f627d75e1cc78b482b4a14d19e5394a1124
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35714167"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const forward = {
  ToRecipients:[
      {
        emailAddress: {
          address:"danas@contoso.onmicrosoft.com",
          name:"Dana Swope"
        }
      }
     ],
  Comment: "Dana, hope you can make this meeting." 
};

let res = await client.api('/me/events/{id}/forward')
    .version('beta')
    .post(forward);

```