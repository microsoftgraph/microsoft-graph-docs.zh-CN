---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a5281154707f25388fc13f73ef20b2f13bdc7cd2
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50784405"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const sendMail = {
  Message: {
    subject: 'Project kickoff',
    toRecipients: [
      {
          emailAddress: {
              name: 'Samantha Booth',
              address: 'samanthab@contoso.onmicrosoft.com'
          }
      }
    ],
    mentions: [
      {
        mentioned: {
          name: 'Dana Swope',
          address: 'danas@contoso.onmicrosoft.com'
         }
      }
    ]
  }
};

await client.api('/me/sendMail')
    .version('beta')
    .post(sendMail);

```