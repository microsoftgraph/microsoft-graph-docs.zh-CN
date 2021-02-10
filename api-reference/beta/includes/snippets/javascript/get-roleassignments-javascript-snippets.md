---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9770b1596e8eeb3723db5e6b0a82585f673bfe94
ms.sourcegitcommit: 48fff935d56fe96e97577a80a3a0aa15c45419ba
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/10/2021
ms.locfileid: "50179284"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/roleManagement/directory/roleAssignments')
    .version('beta')
    .get();

```