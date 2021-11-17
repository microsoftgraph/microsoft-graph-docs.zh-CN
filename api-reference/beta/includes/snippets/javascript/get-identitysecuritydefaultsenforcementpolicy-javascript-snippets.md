---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 291c93542d7a984232983f4be2d629018d07f0db85fafe7fd7dd9d1eb74c8000
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57106024"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let identitySecurityDefaultsEnforcementPolicy = await client.api('/policies/identitySecurityDefaultsEnforcementPolicy')
    .version('beta')
    .get();

```