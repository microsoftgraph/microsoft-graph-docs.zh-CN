---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5a3ab28147c57ed9f9d60b1bf232d1da09ac1a14
ms.sourcegitcommit: c4d6ccd343a6b298a2aa844f1bad66c736487251
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/11/2020
ms.locfileid: "42591654"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/policies/tokenIssuancePolicies')
    .version('beta')
    .get();

```