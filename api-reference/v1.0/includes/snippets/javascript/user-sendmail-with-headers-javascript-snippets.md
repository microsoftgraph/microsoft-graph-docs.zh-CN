---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6a9d980a2188a32013dac9fb4eac17fc49651cac
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50800747"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const sendMail = {
  message: {
    subject: '9/9/2018: concert',
    body: {
      contentType: 'HTML',
      content: 'The group represents Nevada.'
    },
    toRecipients: [
      {
        emailAddress: {
          address: 'AlexW@contoso.OnMicrosoft.com'
        }
      }
    ],
    internetMessageHeaders: [
      {
        name: 'x-custom-header-group-name',
        value: 'Nevada'
      },
      {
        name: 'x-custom-header-group-id',
        value: 'NV001'
      }
    ]
  }
};

await client.api('/me/sendMail')
    .post(sendMail);

```