---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: dbc9aef2e70e778236fc2c344ddecc9ee51cf0f8
ms.sourcegitcommit: be796d6a7ae62f052c381d20207545f057b184d9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/14/2020
ms.locfileid: "48460331"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/policies/permissionGrantPolicies/my-custom-consent-policy/excludes/6a846635-3e70-4a10-821e-512a0db93cbd')
    .version('beta')
    .delete();

```