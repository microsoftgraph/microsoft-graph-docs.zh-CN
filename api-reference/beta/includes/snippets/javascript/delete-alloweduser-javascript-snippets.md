---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1888ec40f1f3a8588b90b96a2e39ab2f2962433d
ms.sourcegitcommit: 33ffed5b785abf36b1a7786856c9266958830d25
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/25/2020
ms.locfileid: "42948060"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/print/printers/{id}/allowedUsers/{id}/$ref')
    .version('beta')
    .delete();

```