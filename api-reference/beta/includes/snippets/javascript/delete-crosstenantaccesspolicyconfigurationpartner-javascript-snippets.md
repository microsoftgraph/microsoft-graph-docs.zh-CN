---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2b71ab990f38ac371ec94c46eeccece1b5466e82
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/08/2022
ms.locfileid: "63335771"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/policies/crossTenantAccessPolicy/partners/9c5d131d-b1c3-4fc4-9e3f-c6557947d551')
    .version('beta')
    .delete();

```