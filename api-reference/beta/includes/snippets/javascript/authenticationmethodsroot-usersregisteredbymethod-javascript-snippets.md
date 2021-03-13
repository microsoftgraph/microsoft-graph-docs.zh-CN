---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6359f653bfbb5e4ef351982b995b01d1c9f1db22
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50807132"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let userRegistrationMethodSummary = await client.api('/reports/authenticationMethods/usersRegisteredByMethod(includedUserTypes='all',includedUserRoles='all')')
    .version('beta')
    .get();

```