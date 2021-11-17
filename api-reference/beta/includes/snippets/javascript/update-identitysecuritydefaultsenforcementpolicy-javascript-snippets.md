---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a73819f30bbf8aefb129a7cc0e6ded137fd81b96c3c2284fad9284e7bb6e8703
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57215840"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const identitySecurityDefaultsEnforcementPolicy = {
  isEnabled: false
};

await client.api('/policies/identitySecurityDefaultsEnforcementPolicy')
    .version('beta')
    .update(identitySecurityDefaultsEnforcementPolicy);

```