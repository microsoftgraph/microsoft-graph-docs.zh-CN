---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 91c39bd1ad06dadddc38ce6ac5f429fe579fd01e
ms.sourcegitcommit: 1a84f80798692fc0381b1acecfe023b3ce6ab02c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/12/2020
ms.locfileid: "41956407"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const subscription = {
   changeType: "updated",
   notificationUrl: "https://webhook.azurewebsites.net/api/send/myNotifyClient",
   resource: "me/mailFolders('Inbox')/messages",
   expirationDateTime:"2016-11-20T18:23:45.9356913Z",
   clientState: "secretClientValue",
   latestSupportedTlsVersion: "v1_2"
};

let res = await client.api('/subscriptions')
    .post(subscription);

```