---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5734a0d05bdca25c290876153dca92267e577a6e
ms.sourcegitcommit: be796d6a7ae62f052c381d20207545f057b184d9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/14/2020
ms.locfileid: "48460252"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/policies/permissionGrantPolicies/my-custom-consent-policy')
    .version('beta')
    .delete();

```