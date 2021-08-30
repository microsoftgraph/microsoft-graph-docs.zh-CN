---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: afe19a96a536530a9387f909b3c13a0c2d475679be1e915c82db136fb1d1f8c9
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57378357"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let appRoleAssignments = await client.api('/users/cdb555e3-b33e-4fd5-a427-17fadacbdfa7/appRoleAssignments')
    .version('beta')
    .filter('resourceId eq 8e881353-1735-45af-af21-ee1344582a4d')
    .get();

```