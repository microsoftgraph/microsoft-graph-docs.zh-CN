---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ff834899b70b240d66bb98d83fbf30e7ced720fc676ef9d8b6e3e70330050fad
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57328991"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let homeRealmDiscoveryPolicies = await client.api('/servicePrincipals/{id}/homeRealmDiscoveryPolicies')
    .version('beta')
    .get();

```