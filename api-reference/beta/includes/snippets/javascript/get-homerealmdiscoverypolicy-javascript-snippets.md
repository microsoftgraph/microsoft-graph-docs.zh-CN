---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2967d5d50c04283ce424032c2d9428e6eaf415c8b0e5de91cea9a385f6f4ab7d
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57215631"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let homeRealmDiscoveryPolicy = await client.api('/policies/homeRealmDiscoveryPolicies/{id}')
    .version('beta')
    .get();

```