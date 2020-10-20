---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d00d7b88b968bd642d9b1a48bc5d164c550f405f
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/20/2020
ms.locfileid: "48619870"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/servicePrincipals/{id}/synchronization/jobs/')
    .version('beta')
    .get();

```