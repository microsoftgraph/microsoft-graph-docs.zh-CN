---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7090fa47c6d4926da9f855cfc6d93dfeeeac4202
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50803149"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let delta = await client.api('/administrativeUnits/delta')
    .version('beta')
    .get();

```