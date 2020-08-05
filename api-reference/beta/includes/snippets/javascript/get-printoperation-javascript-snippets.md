---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6af2bf4251938d171fd47412b271f5107d0cb020
ms.sourcegitcommit: 496410c1e256aa093eabf27f17e820d9ee91a293
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2020
ms.locfileid: "46565625"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/print/operations/{id}')
    .version('beta')
    .get();

```