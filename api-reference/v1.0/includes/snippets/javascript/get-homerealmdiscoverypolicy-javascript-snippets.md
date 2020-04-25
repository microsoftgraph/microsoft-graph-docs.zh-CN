---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9ab31b14411f428b842e25c43f1a4596f1874657
ms.sourcegitcommit: 5575e6607817ba23ceb0b01e2f5fc81e58bdcd1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/22/2020
ms.locfileid: "43805583"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/policies/homeRealmDiscoveryPolicies/{id}')
    .get();

```