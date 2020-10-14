---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 55f4cbd7e5ad45da8630b6be81f72a7ed08697fd
ms.sourcegitcommit: be796d6a7ae62f052c381d20207545f057b184d9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/14/2020
ms.locfileid: "48458601"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/servicePrincipals/{id}/delegatedPermissionClassifications/{id}')
    .version('beta')
    .delete();

```