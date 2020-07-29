---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c2f62ccf743f9e444be9574768c307f266012523
ms.sourcegitcommit: 9faca60f0cc4ee9d6dce33fd25c72e14b5487d34
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/29/2020
ms.locfileid: "46512270"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const subscription = {
   changeType: "created",
   notificationUrl: "https://webhook.azurewebsites.net/api/send/myNotifyClient",
   resource: "me/mailFolders('Inbox')/messages",
   expirationDateTime:"2016-11-20T18:23:45.9356913Z",
   clientState: "secretClientValue",
   latestSupportedTlsVersion: "v1_2"
};

let res = await client.api('/subscriptions')
    .version('beta')
    .post(subscription);

```