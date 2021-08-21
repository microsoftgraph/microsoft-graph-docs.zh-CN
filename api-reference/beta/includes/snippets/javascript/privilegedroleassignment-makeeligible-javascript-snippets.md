---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 256461e0da34bc7f9e2e1596e9e776c3300dd63faf03298a81c69d6995d291bc
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57328750"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/privilegedRoleAssignments/{id}/makeEligible')
    .version('beta')
    .post();

```