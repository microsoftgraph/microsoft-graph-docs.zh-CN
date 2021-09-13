---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: deeb047db5d40e5f09206eb157c2cdc0aa312b19ba924203f3c9369e50a53b5f
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57278192"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const tokenLifetimePolicy = {
  definition: [
    'definition-value'
  ],
  displayName: 'displayName-value',
  isOrganizationDefault: true
};

await client.api('/policies/tokenLifetimePolicies/{id}')
    .update(tokenLifetimePolicy);

```