---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: dc09c883de8aec2916928dc6c702cd359f363662
ms.sourcegitcommit: 33ffed5b785abf36b1a7786856c9266958830d25
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/25/2020
ms.locfileid: "42947828"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const printIdentity = {
  @odata.id: "https://graph.microsoft.com/beta/groups/{id}"
};

let res = await client.api('/print/printers/{id}/allowedGroups/$ref')
    .version('beta')
    .post(printIdentity);

```