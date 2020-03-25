---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 83873ac2eed96cfd05d8a5fabd72301638ca8f1c
ms.sourcegitcommit: 33ffed5b785abf36b1a7786856c9266958830d25
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/25/2020
ms.locfileid: "42947865"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/print/printers/{id}/connectors')
    .version('beta')
    .get();

```