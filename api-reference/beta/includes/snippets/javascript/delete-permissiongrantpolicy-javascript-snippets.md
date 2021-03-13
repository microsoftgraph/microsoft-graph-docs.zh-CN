---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4ff789832ead09249ff26d936ee2623e7448cc90
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50783833"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/policies/permissionGrantPolicies/my-custom-consent-policy')
    .version('beta')
    .delete();

```