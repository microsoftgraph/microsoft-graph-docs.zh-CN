---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e1ac1d4ef26303ac3c814b6cac1168c92b070540
ms.sourcegitcommit: 33ffed5b785abf36b1a7786856c9266958830d25
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/25/2020
ms.locfileid: "42947753"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/print/printers/{id}/resetDefaults')
    .version('beta')
    .post();

```