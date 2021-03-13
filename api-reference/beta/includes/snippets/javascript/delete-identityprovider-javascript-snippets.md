---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 61a277dfe76b2539fb1d4209f470393fe004c812
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50797782"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/identityProviders/{id}')
    .version('beta')
    .delete();

```