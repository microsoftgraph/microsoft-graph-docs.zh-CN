---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 49958ea62c51b1e100182e6fd726accc896b5918
ms.sourcegitcommit: 496410c1e256aa093eabf27f17e820d9ee91a293
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2020
ms.locfileid: "46567242"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const identitySecurityDefaultsEnforcementPolicy = {
  isEnabled: false
};

let res = await client.api('/policies/identitySecurityDefaultsEnforcementPolicy')
    .update(identitySecurityDefaultsEnforcementPolicy);

```