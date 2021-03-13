---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 42616594947e70638b53e3490ae54bb461bc6ee5
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50794953"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let activityStatistics = await client.api('/me/analytics/activitystatistics')
    .version('beta')
    .get();

```