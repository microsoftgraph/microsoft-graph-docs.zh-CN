---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3b4f2758b5f4fd343128ebf09a8426bef1e97d9c
ms.sourcegitcommit: 36bae3615df41876493b25da478e589d1974f97b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/29/2021
ms.locfileid: "59995974"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let simulations = await client.api('/security/attackSimulation/simulations')
    .version('beta')
    .get();

```