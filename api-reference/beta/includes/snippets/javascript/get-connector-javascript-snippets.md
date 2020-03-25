---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 833cf9298b5f7a77dbcf86447d58fb0b08e03a01
ms.sourcegitcommit: 33ffed5b785abf36b1a7786856c9266958830d25
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/25/2020
ms.locfileid: "42948145"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/print/connectors/{id}')
    .version('beta')
    .get();

```