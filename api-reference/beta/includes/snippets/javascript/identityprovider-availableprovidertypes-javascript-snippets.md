---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2c8b1d71aeab48ba07c119b3a6009c1c0d8d9584
ms.sourcegitcommit: 496410c1e256aa093eabf27f17e820d9ee91a293
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2020
ms.locfileid: "46566771"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/identityProviders/availableProviderTypes')
    .version('beta')
    .get();

```