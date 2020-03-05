---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2b506cf74a70033cf58e5cbab353ba2a8935b330
ms.sourcegitcommit: 2f78ac96a9b0462626a242429055ef824590bd3f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2020
ms.locfileid: "41558888"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const policy = {
  definition: [
    "definition-value"
  ],
  displayName: "displayName-value",
  isOrganizationDefault: true
};

let res = await client.api('/policies/tokenLifetimePolicies')
    .version('beta')
    .post(policy);

```