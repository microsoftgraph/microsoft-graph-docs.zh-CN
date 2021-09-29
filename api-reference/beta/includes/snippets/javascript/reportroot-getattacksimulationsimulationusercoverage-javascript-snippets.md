---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 95f482ec0a79b2b9e58689bc63c473ae87596ed6
ms.sourcegitcommit: 36bae3615df41876493b25da478e589d1974f97b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/29/2021
ms.locfileid: "59996379"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let getAttackSimulationSimulationUserCoverage = await client.api('/reports/getAttackSimulationSimulationUserCoverage')
    .version('beta')
    .get();

```