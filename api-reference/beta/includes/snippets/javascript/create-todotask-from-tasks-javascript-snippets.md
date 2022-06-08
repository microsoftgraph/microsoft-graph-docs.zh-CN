---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 31314e294c79ddb99e5ff7adde5f307685a4e74e
ms.sourcegitcommit: a345f96fb22115f65840702a4acf0acc7c1b0679
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/08/2022
ms.locfileid: "65946825"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const todoTask = {
   title: 'A new task',
   categories: ['Important'],
   linkedResources: [
      {
         webUrl: 'http://microsoft.com',
         applicationName: 'Microsoft',
         displayName: 'Microsoft'
      }
   ]
};

await client.api('/me/todo/lists/AQMkADAwATM0MDAAMS0yMDkyLWVjMzYtM/tasks')
    .version('beta')
    .post(todoTask);

```