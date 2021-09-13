---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 37161787bb1cfa9424dbfeb4b7b66c052e204bcf3c560e0e65148510e737755e
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57277549"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const claimsMappingPolicy = {
  definition: [
    'definition-value'
  ],
  displayName: 'displayName-value',
  isOrganizationDefault: true
};

await client.api('/policies/claimsMappingPolicies')
    .post(claimsMappingPolicy);

```