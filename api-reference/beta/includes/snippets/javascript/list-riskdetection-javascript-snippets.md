---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 98a84e281bb19f0ffa8b1ae3928aaddd32b78eac
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50781160"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let riskDetection = await client.api('/identityProtection/riskDetections/c2b6c2b9-dddc-acd0-2b39-d519d803dbc3')
    .version('beta')
    .get();

```