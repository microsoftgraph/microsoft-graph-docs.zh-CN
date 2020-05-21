---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 09a0c1838c873ef5dc2b4c4a3c405cbdd93e8279
ms.sourcegitcommit: 5a1373f2ccd9ee813fc60d42e7ac6b115b5f9f66
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/21/2020
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