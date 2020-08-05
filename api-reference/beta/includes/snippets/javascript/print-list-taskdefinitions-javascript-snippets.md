---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4b04d095b644d5f3d91919121de80bafdb819de2
ms.sourcegitcommit: 496410c1e256aa093eabf27f17e820d9ee91a293
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2020
ms.locfileid: "46566442"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/print/taskDefinitions')
    .version('beta')
    .get();

```