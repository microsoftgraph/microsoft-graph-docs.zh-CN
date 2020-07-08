---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 23873b5a163275cdc43713e9f65c2211cf54aa8f
ms.sourcegitcommit: 2050639c9e9a6b2dab9ce53d6a9fc87e98789b50
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/08/2020
ms.locfileid: "45081719"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/roleManagement/directory/roleAssignments')
    .version('beta')
    .filter(' principalId eq 'f1847572-48aa-47aa-96a3-2ec61904f41f'')
    .get();

```