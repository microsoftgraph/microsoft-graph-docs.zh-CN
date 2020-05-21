---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9d090671f07a81f4b532efd13f33f61c5d231969
ms.sourcegitcommit: 5a1373f2ccd9ee813fc60d42e7ac6b115b5f9f66
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/21/2020
ms.locfileid: "44332683"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/insights/used')
    .version('beta')
    .get();

```