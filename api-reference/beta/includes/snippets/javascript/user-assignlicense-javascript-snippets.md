---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 624505f5a1fb98a60bb66d450001f2eb8c121a022d703d9908f2f9a6ab440bd0
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57163758"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const user = {
  addLicenses: [
    {
      disabledPlans: [ '11b0131d-43c8-4bbb-b2c8-e80f9a50834a' ],
      skuId: 'skuId-value-1'
    },
    {
      disabledPlans: [ 'a571ebcc-fqe0-4ca2-8c8c-7a284fd6c235' ],
      skuId: 'skuId-value-2'
    }
  ],
  removeLicenses: []
};

await client.api('/me/assignLicense')
    .version('beta')
    .post(user);

```