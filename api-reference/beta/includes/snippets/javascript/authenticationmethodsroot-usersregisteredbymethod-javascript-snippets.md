---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4c9baf1ba3297e6f7bb96fb54e10d74ef194ad6ecbd31da39a864d2864b88bb8
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57105062"
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