---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 89496baa1e4079c87acc7c04cf0391606b2b41fdc77cd032b90fa1f47ceb85b7
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57279766"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/servicePrincipals/{id}/homeRealmDiscoveryPolicies/{id}/$ref')
    .delete();

```