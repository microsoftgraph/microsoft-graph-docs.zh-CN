---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3308ccf2ea9258beaae5133cf195760830ba4bb4
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/08/2022
ms.locfileid: "63337360"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let riskyServicePrincipals = await client.api('/identityProtection/riskyServicePrincipals')
    .version('beta')
    .get();

```