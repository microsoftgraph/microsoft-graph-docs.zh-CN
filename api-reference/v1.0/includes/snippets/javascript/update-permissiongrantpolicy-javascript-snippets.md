---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 32e9df2e09d0308c3b7d63e6b0af07dd38e525ca8afad90b2fb3644dea1c2f11
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57220546"
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
    .update(permissionGrantPolicy);

```