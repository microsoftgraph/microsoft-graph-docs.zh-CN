---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2b95cf2b7ab154841861d5f82ac3d6d5aa2d0492
ms.sourcegitcommit: 9f88b7e41a4a4a4d5f52bd995ce07c6f702bd5d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/01/2020
ms.locfileid: "49523997"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/servicePrincipals/{id}/delegatedPermissionClassifications')
    .get();

```