---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 08d80b6501462d45469f7d73de5bf45f10154b1b73b9835d72aedb39637c9740
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57278028"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/privilegedRoleAssignmentRequests/7c53453e-d5a4-41e0-8eb1-32d5ec8bfdee/cancel')
    .version('beta')
    .post();

```