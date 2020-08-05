---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 33abb9591c2fcc91e827e6d6012aa2cff2d7702a
ms.sourcegitcommit: 496410c1e256aa093eabf27f17e820d9ee91a293
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2020
ms.locfileid: "46570027"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/identityProtection/riskyUsers')
    .version('beta')
    .get();

```