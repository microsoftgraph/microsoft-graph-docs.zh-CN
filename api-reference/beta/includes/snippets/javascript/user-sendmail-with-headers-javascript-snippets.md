---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c80f96ec9a0e6e3fbfb1ce750c54bbe90a4fdbaccde523520bd8e1638ec75cc4
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57220064"
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
    .version('beta')
    .post(sendMail);

```