---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 04b7cfa60fdada75c5b78287ad2af09d2c9395b3
ms.sourcegitcommit: 69c355eeb620b76ca70d896f984e21c32ac09eb0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2021
ms.locfileid: "50092334"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/reports/authenticationMethods/usersRegisteredByFeature(includedUserTypes='all',includedUserRoles='all')')
    .version('beta')
    .get();

```