---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7eda83026bdf0d1d74145e1e446747930b9ba4bb
ms.sourcegitcommit: a1675c7b8dfc7d7c3c7923d06cda2b0127f9c3e6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/05/2021
ms.locfileid: "49754163"
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
    .post(forward);

```