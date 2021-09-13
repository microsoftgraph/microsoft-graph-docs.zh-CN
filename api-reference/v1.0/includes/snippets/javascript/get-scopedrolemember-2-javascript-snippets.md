---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6cb9799a4dad1057f7a71edabf0a110bed12fd4f68bb2873cb3ea30589a23398
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57221456"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let scopedRoleMembers = await client.api('/directory/administrativeUnits/{id}/scopedRoleMembers')
    .get();

```