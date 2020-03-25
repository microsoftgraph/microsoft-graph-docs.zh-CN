---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: bc667727927df96045149beb986ea1cce286d732
ms.sourcegitcommit: 33ffed5b785abf36b1a7786856c9266958830d25
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/25/2020
ms.locfileid: "42948255"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/print/services')
    .version('beta')
    .get();

```