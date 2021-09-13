---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: df4a432516eaded193a197a960feb763811805d3f49d6ac77cf6998888545618
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57104269"
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