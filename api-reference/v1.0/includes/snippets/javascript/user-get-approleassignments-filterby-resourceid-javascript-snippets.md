---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e70ca9a0ea5a2219c2293b03d0204d27acfc3edd
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50777424"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let appRoleAssignments = await client.api('/users/cdb555e3-b33e-4fd5-a427-17fadacbdfa7/appRoleAssignments')
    .filter('resourceId eq 8e881353-1735-45af-af21-ee1344582a4d')
    .get();

```