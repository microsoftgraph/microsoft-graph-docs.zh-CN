---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9e77237c4ad4119169d99159c0ef8d4be99de405070397f4dcb5742ffa78ec24
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57278530"
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

await client.api('/policies/homeRealmDiscoveryPolicies/{id}')
    .update(homeRealmDiscoveryPolicy);

```