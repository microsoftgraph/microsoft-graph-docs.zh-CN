---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e1e4f50e9a03fe6a85fba9d15818be3204b66f583de1237bb49e2615a86aa39f
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57221076"
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