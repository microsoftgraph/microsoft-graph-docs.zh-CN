---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c9a10ffded972252ad09c1abbdd1f95c7bc24380
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50796704"
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
    .post(todoTask);

```