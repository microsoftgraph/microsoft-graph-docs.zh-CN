---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: bdb5207b84a9c8c2f46b81123fe598ab81a3f09a4d27cdd6858ac9b1fab6c37f
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57161190"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const permissionGrantPolicy = {
  displayName: 'Custom permission grant policy'
};

await client.api('/policies/permissionGrantPolicies/my-custom-consent-policy')
    .version('beta')
    .update(permissionGrantPolicy);

```