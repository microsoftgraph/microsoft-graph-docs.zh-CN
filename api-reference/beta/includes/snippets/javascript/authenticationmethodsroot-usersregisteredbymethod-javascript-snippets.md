---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ebea3e2e8b25092cc0543575f06be406d4853306
ms.sourcegitcommit: 69c355eeb620b76ca70d896f984e21c32ac09eb0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2021
ms.locfileid: "50092367"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/reports/authenticationMethods/usersRegisteredByMethod(includedUserTypes='all',includedUserRoles='all')')
    .version('beta')
    .get();

```