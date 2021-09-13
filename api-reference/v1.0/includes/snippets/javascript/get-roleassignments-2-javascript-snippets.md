---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: bfb5a3f700034608d92b1ef7a8343abade80399b
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59130414"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let roleAssignments = await client.api('/roleManagement/directory/roleAssignments')
    .filter(' principalId eq \'f1847572-48aa-47aa-96a3-2ec61904f41f\'')
    .get();

```