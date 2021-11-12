---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: cbf7be080993170ad789f09024be3005528f4b4274ffb34789593b978d522425
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57163653"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let printTaskTrigger = await client.api('/print/printers/{printerId}/taskTriggers/{taskTriggerId}')
    .version('beta')
    .get();

```