---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 62faea24efbdaeb94010619fa8d5c9d0a997ce75
ms.sourcegitcommit: 9f88b7e41a4a4a4d5f52bd995ce07c6f702bd5d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/01/2020
ms.locfileid: "49522382"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const sendActivityNotification = {
    topic: {
        source: "entityUrl",
        value: "https://graph.microsoft.com/beta/users/{userId}/teamwork/installedApps/{installationId}"
    },
    activityType: "taskCreated",
    previewText: {
        content: "New Task Created"
    },
    templateParameters: [
        {
            name: "taskId",
            value: "Task 12322"
        }
    ]
};

let res = await client.api('/users/{userId}/teamwork/sendActivityNotification')
    .version('beta')
    .post(sendActivityNotification);

```