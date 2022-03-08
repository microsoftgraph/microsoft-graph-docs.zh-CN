---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 36329004b274824586fd82fb00234da526047a20
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/08/2022
ms.locfileid: "63336429"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/policies/crossTenantAccessPolicy/default/resetToSystemDefault')
    .version('beta')
    .post();

```