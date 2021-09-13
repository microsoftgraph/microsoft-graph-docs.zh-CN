---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4679f8229bd76fd088dd6e76e2bcaf3e47722cba905dc442fdaf011ea4f35104
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56904083"
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