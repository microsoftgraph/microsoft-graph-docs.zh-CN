---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e909f04a515d137850af02a32929353d18618c73
ms.sourcegitcommit: 496410c1e256aa093eabf27f17e820d9ee91a293
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2020
ms.locfileid: "46565895"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/print/printers/{id}/taskTriggers')
    .version('beta')
    .get();

```