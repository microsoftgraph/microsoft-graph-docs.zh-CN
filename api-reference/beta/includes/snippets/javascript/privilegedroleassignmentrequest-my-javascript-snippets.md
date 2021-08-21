---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 20f182e2c370ea49180c68f5bfec7debd43a82909eca2296358688b4aebe70e3
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57219712"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let my = await client.api('/privilegedRoleAssignmentRequests/my')
    .version('beta')
    .get();

```