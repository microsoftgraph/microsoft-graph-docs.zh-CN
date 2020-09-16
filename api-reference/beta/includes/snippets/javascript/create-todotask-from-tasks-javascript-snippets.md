---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6fe8e2cfe9209894841be22912d8f84e5e724537
ms.sourcegitcommit: 7e1993d64cc6d3145ae0ca984fefe74772b6052b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/16/2020
ms.locfileid: "47843035"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const todoTask = {
  title:"A new task",
  linkedResources: [{
            webUrl: "http://microsoft.com",
            applicationName: "Microsoft",
            displayName: "Microsoft"
        }]
};

let res = await client.api('/me/todo/lists/AQMkADAwATM0MDAAMS0yMDkyLWVjMzYtM/tasks')
    .version('beta')
    .post(todoTask);

```