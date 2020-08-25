---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e781e5418c01fd411336376df490c2f088e1dc78
ms.sourcegitcommit: ef47b165f7a140cfc0309a275cb8722dd265660d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/25/2020
ms.locfileid: "46873131"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const tasks = {
  title:"A new task",
  linkedResources: [{
            webUrl: "http://microsoft.com",
            applicationName: "Microsoft",
            displayName: "Microsoft"
        }]
};

let res = await client.api('/me/todo/lists/AQMkADAwATM0MDAAMS0yMDkyLWVjMzYtM/tasks')
    .version('beta')
    .post(tasks);

```