---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 19fddccb9a75f766684c61480bc018049d878c4d
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50792416"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let tokenLifetimePolicy = await client.api('/policies/tokenLifetimePolicies/{id}')
    .version('beta')
    .get();

```