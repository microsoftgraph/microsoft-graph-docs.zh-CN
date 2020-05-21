---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2c34223f84cf07dca6e00267a04af27129752e2d
ms.sourcegitcommit: 5a1373f2ccd9ee813fc60d42e7ac6b115b5f9f66
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/21/2020
ms.locfileid: "44338957"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/policies/tokenIssuancePolicies/{id}')
    .version('beta')
    .get();

```