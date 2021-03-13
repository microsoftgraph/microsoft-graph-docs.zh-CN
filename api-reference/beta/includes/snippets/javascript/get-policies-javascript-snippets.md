---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0a6cf27cd569441408565218c0e383ad1b323d4e
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50796690"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let policies = await client.api('/identity/conditionalAccess/policies')
    .version('beta')
    .filter('displayName eq \'SimplePolicy1\' or displayName eq \'SimplePolicy2\'')
    .get();

```