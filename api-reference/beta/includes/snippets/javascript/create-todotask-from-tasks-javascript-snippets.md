---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3f5be596a5c258c364b6ef8c3bd9ac69b83db0f3f5c4f60a1f987ef62a26ee89
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56903634"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const todoTask = {
   title: 'A new task',
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