---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b980af4e60cb5217a3653e45da867bb31af0f9a9b47f06d5795445d6a69b1da9
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57164194"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let riskyUsers = await client.api('/tenantRelationships/managedTenants/riskyUsers')
    .version('beta')
    .get();

```