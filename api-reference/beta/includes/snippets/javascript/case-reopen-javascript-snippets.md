---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5a48d514f36a2be8163bdc88f2b0b4c1468a98c8
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50773709"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/compliance/ediscovery/cases/061b9a92-8926-4bd9-b41d-abf35edc7583/reopen')
    .version('beta')
    .post();

```