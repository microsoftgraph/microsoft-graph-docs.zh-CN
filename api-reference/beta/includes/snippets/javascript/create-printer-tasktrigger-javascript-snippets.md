---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: de9d2ee1284542039988bc1983338d611820091b
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50792396"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const printTaskTrigger = {
  event: 'jobStarted',
  'definition@odata.bind': 'https://graph.microsoft.com/beta/print/taskDefinitions/3203656e-6069-4e10-8147-d25290b00a3c'
};

await client.api('/print/printers/ae63f617-4856-4b45-8ea9-69dfbeea230e/taskTriggers')
    .version('beta')
    .post(printTaskTrigger);

```