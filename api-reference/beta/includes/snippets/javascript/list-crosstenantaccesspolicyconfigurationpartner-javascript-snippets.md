---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ba60670c394e90b727e586567114d30237b0e6c0
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/08/2022
ms.locfileid: "63336541"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let partners = await client.api('/policies/crossTenantAccessPolicy/partners')
    .version('beta')
    .get();

```