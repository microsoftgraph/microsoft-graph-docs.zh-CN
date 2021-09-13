---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d5472b7dbb47128a0cdcf89f9dd7a0d8c5fb19a5290145dff3f90ee39c3ec959
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57161971"
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