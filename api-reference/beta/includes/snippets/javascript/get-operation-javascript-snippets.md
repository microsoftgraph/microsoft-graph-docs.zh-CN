---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1204873fb08d127a11b27554cfa431e846026d0c
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50798164"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let longRunningOperation = await client.api('/users/{id | userPrincipalName}/authentication/operations/{id}')
    .version('beta')
    .get();

```