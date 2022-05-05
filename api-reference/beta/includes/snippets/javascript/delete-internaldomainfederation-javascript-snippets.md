---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d4ac556c0ac0271583c1531ddd225440f4c3e0bc
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65211773"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/domains/contoso.com/federationConfiguration/96db02e2-80c1-5555-bc3a-de92ffb8c5be')
    .version('beta')
    .delete();

```