---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6aebe1cb9ebdd032f6ef4f7a1e795fe2702ef0fe597aef74982cc0d95bfa12c3
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57278767"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let includes = await client.api('/policies/permissionGrantPolicies/microsoft-application-admin/includes')
    .version('beta')
    .get();

```