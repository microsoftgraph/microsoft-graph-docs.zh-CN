---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: fc06446031dd6f64d5523b3b71c780fa1242d6fe
ms.sourcegitcommit: 08d47a31c48fd69ae4fcee26e34fdd65ad1ba69f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/02/2021
ms.locfileid: "51507469"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/teams/57fb72d0-d811-46f4-8947-305e6072eaa5/completeMigration')
    .version('beta')
    .post();

```