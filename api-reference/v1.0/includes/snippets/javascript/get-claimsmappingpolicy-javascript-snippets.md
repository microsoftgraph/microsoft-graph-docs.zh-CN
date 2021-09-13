---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 11ace6aea97c906e7d5e34c581962de5d1198cf3e06ee7bc843b9460bdf0bff9
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57106811"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let claimsMappingPolicy = await client.api('/policies/claimsMappingPolicies/{id}')
    .get();

```