---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c88e83b10b3d4731f9094714ba6aa5923f60d094
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50780202"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/external/connections/contosohr/groups/31bea3d537902000')
    .version('beta')
    .delete();

```