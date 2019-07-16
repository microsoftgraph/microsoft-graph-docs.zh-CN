---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 07d361280e02243ee45c6bc03d76ae2e827007c8
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35738336"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const subscription = {
   changeType: "created,updated",
   notificationUrl: "https://webhook.azurewebsites.net/api/send/myNotifyClient",
   resource: "me/mailFolders('Inbox')/messages",
   expirationDateTime:"2016-11-20T18:23:45.9356913Z",
   clientState: "secretClientValue"
};

let res = await client.api('/subscriptions')
    .post({subscription : subscription});

```