---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d54c19848c6a2f79b2af72a9ac08a4eefc298efd73119f86e5e8d8e7bcb8dce6
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57328999"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let privilegedRoleAssignmentRequests = await client.api('/privilegedRoleAssignmentRequests')
    .version('beta')
    .get();

```