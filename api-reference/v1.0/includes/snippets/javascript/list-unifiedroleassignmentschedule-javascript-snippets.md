---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a8ed2320a80721beb529d2ac9db6c961642c32b1
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65207192"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let roleAssignmentSchedules = await client.api('/roleManagement/directory/roleAssignmentSchedules')
    .get();

```