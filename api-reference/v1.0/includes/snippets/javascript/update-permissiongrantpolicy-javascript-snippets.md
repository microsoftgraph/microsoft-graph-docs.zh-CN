---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9810f5912e7007298d8f3a04171cab1a63203b55
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50784732"
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