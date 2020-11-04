---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 10441aa13a01d1b3f77eb5a5b60c39542986fa0d
ms.sourcegitcommit: 82da4012294b046416c9ae93d2294d80dab217f6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/04/2020
ms.locfileid: "48904433"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const todoTask = {
   title:"A new task",
   linkedResources:[
      {
         webUrl:"http://microsoft.com",
         applicationName:"Microsoft",
         displayName:"Microsoft"
      }
   ]
};

let res = await client.api('/me/todo/lists/AQMkADAwATM0MDAAMS0yMDkyLWVjMzYtM/tasks')
    .post(todoTask);

```