---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: fc6cdcdb64bc4d66449bc4313484b42145705a86
ms.sourcegitcommit: 0329bbcd5f1b09a2a6c5f935a30c4560b6eed492
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/27/2019
ms.locfileid: "36636739"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const message = {
    subject:"9/8/2018: concert",
    body:{
        contentType:"HTML",
        content:"The group represents Washington."
    },
    toRecipients:[
        {
            emailAddress:{
                address:"AlexW@contoso.OnMicrosoft.com"
            }
        }
    ],
    internetMessageHeaders:[
        {
            name:"x-custom-header-group-name",
            value:"Washington"
        },
        {
            name:"x-custom-header-group-id",
            value:"WA001"
        }
    ]
};

let res = await client.api('/me/messages')
    .post(message);

```