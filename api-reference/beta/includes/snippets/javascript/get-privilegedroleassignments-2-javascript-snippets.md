---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c93577635fb92d13a2713caf160c9f7e70ffe8074b5c4c4ea2c5fb752bfbca96
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57273956"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let privilegedRoleAssignments = await client.api('/privilegedRoleAssignments')
    .version('beta')
    .filter('isElevated eq true')
    .get();

```