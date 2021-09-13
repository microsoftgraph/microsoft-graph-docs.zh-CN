---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9f9650f1dc9951da37fde9ec68b56ead48e229b6dd524eed65b54d8563d860ed
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57334054"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const servicePrincipal = {
  appRoleAssignmentRequired: true
};

await client.api('/servicePrincipals/{id}')
    .update(servicePrincipal);

```