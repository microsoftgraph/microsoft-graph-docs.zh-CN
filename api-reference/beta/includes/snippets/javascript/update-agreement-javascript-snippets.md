---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1a88ab1d73ac4bef122ecc344f3c1439fda642ea
ms.sourcegitcommit: 0bcc0a93f37db6013be40dc8d36717aeeeef7fb6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/16/2022
ms.locfileid: "63528088"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const agreement = {
    displayName: 'All Contoso volunteers - Terms of use',
    isViewingBeforeAcceptanceRequired: true
};

await client.api('/identityGovernance/termsOfUse/agreements/0ec9f6a6-159d-4dd8-a563-1f0b5935e80b')
    .version('beta')
    .update(agreement);

```