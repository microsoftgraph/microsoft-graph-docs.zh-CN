---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c4ef511be66c5c70abe2d84b297515f6664e50b3
ms.sourcegitcommit: 33ffed5b785abf36b1a7786856c9266958830d25
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/25/2020
ms.locfileid: "42947779"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/print/printers/{id}/jobs')
    .version('beta')
    .post();

```