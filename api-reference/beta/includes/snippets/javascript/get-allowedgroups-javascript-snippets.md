---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8e9c5a417f61260a3ebddc8255aecc2174e0a4bd
ms.sourcegitcommit: 33ffed5b785abf36b1a7786856c9266958830d25
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/25/2020
ms.locfileid: "42947921"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/print/printers/{id}/allowedGroups')
    .version('beta')
    .get();

```