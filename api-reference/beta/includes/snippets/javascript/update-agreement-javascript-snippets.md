---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3136d3a6ce832d5de6f118e71fa6acfebc7a0097
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50773905"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const agreement = {
  displayName: 'displayName-value',
  isViewingBeforeAcceptanceRequired: true
};

await client.api('/identityGovernance/termsOfUse/agreements/{id}')
    .version('beta')
    .update(agreement);

```