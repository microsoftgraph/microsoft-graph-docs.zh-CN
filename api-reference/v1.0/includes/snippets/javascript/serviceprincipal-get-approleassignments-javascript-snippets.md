---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 232ea0ee38ac8014c25d0820c33dd8933b47d61debc0afac96e5254347c97076
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57161996"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let appRoleAssignments = await client.api('/servicePrincipals/8e881353-1735-45af-af21-ee1344582a4d/appRoleAssignments')
    .get();

```