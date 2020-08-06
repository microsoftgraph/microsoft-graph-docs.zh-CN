---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c576cd136dd1b149bbdae8c350293eac186586b6
ms.sourcegitcommit: 496410c1e256aa093eabf27f17e820d9ee91a293
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2020
ms.locfileid: "46567274"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/policies/identitySecurityDefaultsEnforcementPolicy')
    .get();

```