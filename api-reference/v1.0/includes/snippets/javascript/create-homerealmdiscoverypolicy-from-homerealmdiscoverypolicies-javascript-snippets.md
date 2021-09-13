---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3cc81269182af69903f19a29d7ac9e1fdf427b341e6c40cca7d3f2c090d295eb
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57332759"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const homeRealmDiscoveryPolicy = {
  definition: [
    'definition-value'
  ],
  displayName: 'displayName-value',
  isOrganizationDefault: true
};

await client.api('/policies/homeRealmDiscoveryPolicies')
    .post(homeRealmDiscoveryPolicy);

```