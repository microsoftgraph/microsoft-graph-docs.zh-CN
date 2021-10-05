---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5bbd6caff7dbcc789d0c0e3725cfafaa59fa645edf836f17d4c07b18865d003a
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57161994"
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
    .post(subscription);

```