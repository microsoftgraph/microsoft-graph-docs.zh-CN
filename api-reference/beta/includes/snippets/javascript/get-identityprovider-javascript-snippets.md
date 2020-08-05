---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3ebcfd385fb5620db611e11d23cfd8f43498cb0e
ms.sourcegitcommit: 496410c1e256aa093eabf27f17e820d9ee91a293
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2020
ms.locfileid: "46566742"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/identityProviders')
    .version('beta')
    .get();

```