---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 43a47078606e0ca1473c042ce34c5518df7bdeb8
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50809232"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let users = await client.api('/users')
    .version('beta')
    .select('displayName,userPrincipalName,signInActivity')
    .get();

```