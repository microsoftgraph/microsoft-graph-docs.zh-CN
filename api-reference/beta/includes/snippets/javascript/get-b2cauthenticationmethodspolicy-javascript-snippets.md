---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 77433e251ad9bde16dc30222b12e7bbcfa58151e
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50792926"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let b2cAuthenticationMethodsPolicy = await client.api('/policies/b2cAuthenticationMethodsPolicy')
    .version('beta')
    .get();

```