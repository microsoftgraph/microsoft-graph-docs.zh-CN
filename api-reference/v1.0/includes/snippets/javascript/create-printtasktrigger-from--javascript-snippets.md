---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e63da2919ed0f522ce75f8c9c4992735467fecc0
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50771825"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const printTaskTrigger = {
  event: 'jobStarted',
  'definition@odata.bind': 'https://graph.microsoft.com/v1.0/print/taskDefinitions/{taskDefinitionId}'
};

await client.api('/print/printers/{printerId}/taskTriggers')
    .post(printTaskTrigger);

```