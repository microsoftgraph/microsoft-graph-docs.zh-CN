---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 99f18c989601325f8f46e164e134d35e145f1564
ms.sourcegitcommit: 5575e6607817ba23ceb0b01e2f5fc81e58bdcd1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/22/2020
ms.locfileid: "43806137"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/reports/getRelyingPartyDetailedSummary(period='period_value')')
    .version('beta')
    .get();

```