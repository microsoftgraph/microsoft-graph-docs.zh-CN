---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 09a0c1838c873ef5dc2b4c4a3c405cbdd93e8279
ms.sourcegitcommit: 94c8985a3956622ea90f7e641f894d57b0982eb9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/02/2020
ms.locfileid: "44338836"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/riskDetections')
    .version('beta')
    .filter('riskEventType eq 'unfamiliarFeatures' or riskLevel eq 'medium'')
    .get();

```