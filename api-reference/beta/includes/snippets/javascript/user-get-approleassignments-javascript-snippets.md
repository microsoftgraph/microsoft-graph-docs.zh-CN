---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 11cffaf1bada8704172ac29fc871e0b409eb73b8420259c819088324879d436f
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57333635"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let appRoleAssignments = await client.api('/users/cdb555e3-b33e-4fd5-a427-17fadacbdfa7/appRoleAssignments')
    .version('beta')
    .get();

```