---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8dd50cf880f37d2dae2a015fcf87faf5ac7d1012
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50805402"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/me/profile/educationalActivities/{id}')
    .version('beta')
    .delete();

```