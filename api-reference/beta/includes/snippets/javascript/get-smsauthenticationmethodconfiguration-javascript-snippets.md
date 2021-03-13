---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2a452351577b37d4597604b49fd2570cc3f05efa
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50799828"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let authenticationMethodConfiguration = await client.api('/policies/authenticationMethodsPolicy/authenticationMethodConfigurations/sms')
    .version('beta')
    .get();

```