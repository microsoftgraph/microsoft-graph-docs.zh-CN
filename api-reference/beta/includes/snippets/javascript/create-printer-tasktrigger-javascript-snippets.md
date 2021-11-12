---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 890727fd18da191ca301eefba137370643ba62d614f804260f5b3b0eb64cb644
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57105544"
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