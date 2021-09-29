---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f6cc85d1ee18b20c77e58cef76faf37701f01f36
ms.sourcegitcommit: 36bae3615df41876493b25da478e589d1974f97b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/29/2021
ms.locfileid: "59995369"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let simulationReportOverview = await client.api('/security/attackSimulation/simulations/{id}/report/overview')
    .version('beta')
    .get();

```