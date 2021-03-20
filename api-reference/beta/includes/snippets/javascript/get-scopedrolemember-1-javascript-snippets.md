---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1309b2c6c31cb9d02e873a65692609c1e2e8deef
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50942997"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let scopedRoleMembership = await client.api('/administrativeUnits/{id}/scopedRoleMembers/{id}')
    .version('beta')
    .get();

```