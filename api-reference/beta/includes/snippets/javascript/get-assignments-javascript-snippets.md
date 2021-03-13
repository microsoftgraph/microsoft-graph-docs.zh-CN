---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 02071b40ca3f65b9364fee1fab1b3c947d9a4921
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50785036"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let assignments = await client.api('/privilegedRoles/{id}/assignments')
    .version('beta')
    .get();

```