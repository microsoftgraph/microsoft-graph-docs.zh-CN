---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3c0574a287c251719bc876249aa009f9ce9c6a59
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65212701"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let runs = await client.api('/security/attackSimulation/simulationAutomations/fbad62b0-b32d-b6ac-9f48-d84bbea08f96/runs')
    .version('beta')
    .get();

```