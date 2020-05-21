---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 291de2d7f8b3f19b60dd879fed442b3930c75025
ms.sourcegitcommit: 5a1373f2ccd9ee813fc60d42e7ac6b115b5f9f66
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/21/2020
ms.locfileid: "44332682"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/insights/used')
    .version('beta')
    .orderby('LastUsed/LastAccessedDateTime')
    .get();

```