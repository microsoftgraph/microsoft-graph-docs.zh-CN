---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 15336aba171bf37095304054d610dd9d8ca1f7ba
ms.sourcegitcommit: 6bb3c5c043d35476e41ef2790bcf4813fae0769d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/15/2022
ms.locfileid: "66096392"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let myRoles = await client.api('/tenantRelationships/managedTenants/myRoles')
    .version('beta')
    .get();

```