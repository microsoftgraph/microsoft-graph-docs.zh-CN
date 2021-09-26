---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 02d7236e31795282f29af6338b9918be901ae401
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59764882"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let roleAssignments = await client.api('/roleManagement/deviceManagement/roleAssignments')
    .version('beta')
    .filter(' principalIds/any(x:x eq \'564ae70c-73d9-476b-820b-fb61eb7384b9\')')
    .get();

```