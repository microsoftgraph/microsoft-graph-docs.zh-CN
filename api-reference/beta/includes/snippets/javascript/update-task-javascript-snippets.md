---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: cb116ef16828cc3cca701a20bc7e13bcc12f34aa
ms.sourcegitcommit: 496410c1e256aa093eabf27f17e820d9ee91a293
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2020
ms.locfileid: "46565236"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const printTask = {
  status: {
    state: "completed",
    description: "completed"
  }
};

let res = await client.api('/print/taskDefinitions/3203656e-6069-4e10-8147-d25290b00a3c/tasks/d036638b-1272-4bba-9227-732463823ed3')
    .version('beta')
    .update(printTask);

```