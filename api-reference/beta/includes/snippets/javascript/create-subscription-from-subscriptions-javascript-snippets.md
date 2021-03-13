---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 29cd06ac46ec0b4191eacef9ed631e31edae31b2
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50803181"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const subscription = {
   changeType: 'created',
   notificationUrl: 'https://webhook.azurewebsites.net/api/send/myNotifyClient',
   resource: 'me/mailFolders(\'Inbox\')/messages',
   expirationDateTime: '2016-11-20T18:23:45.9356913Z',
   clientState: 'secretClientValue',
   latestSupportedTlsVersion: 'v1_2'
};

await client.api('/subscriptions')
    .version('beta')
    .post(subscription);

```