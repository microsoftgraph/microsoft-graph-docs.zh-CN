---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ecd9f7d4eea14e437274c69808ea975946e7c92d
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/20/2020
ms.locfileid: "48609083"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/domains/contoso.com/verify')
    .version('beta')
    .post();

```