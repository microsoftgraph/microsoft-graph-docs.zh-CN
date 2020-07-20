---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d33c203f6b3373f6806b5224474395de16a7138b
ms.sourcegitcommit: 1ec5a7be90790aaebdf6d85d93ab0c72b381c9c3
ms.translationtype: Auto
ms.contentlocale: zh-CN
ms.lasthandoff: 06/24/2020
ms.locfileid: "44863584"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/servicePrincipals/{id}/homeRealmDiscoveryPolicies')
    .get();

```