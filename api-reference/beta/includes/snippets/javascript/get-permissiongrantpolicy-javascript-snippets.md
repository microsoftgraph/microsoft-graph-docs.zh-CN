---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6643348dc7d76fce1ac54168fe3055d9fa2f703f
ms.sourcegitcommit: be796d6a7ae62f052c381d20207545f057b184d9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/14/2020
ms.locfileid: "48460223"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/policies/permissionGrantPolicies/microsoft-user-default-low')
    .version('beta')
    .get();

```