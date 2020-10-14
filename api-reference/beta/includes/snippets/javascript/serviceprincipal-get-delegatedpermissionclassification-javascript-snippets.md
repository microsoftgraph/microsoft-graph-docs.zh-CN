---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4758768308a5001437e7c3b3baef5cdea2de6fb0
ms.sourcegitcommit: be796d6a7ae62f052c381d20207545f057b184d9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/14/2020
ms.locfileid: "48460113"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/servicePrincipals/{id}/delegatedPermissionClassifications')
    .version('beta')
    .get();

```