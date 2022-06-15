---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: de89eeee61e6171ec47453e72c79dca8ee9da972
ms.sourcegitcommit: 6bb3c5c043d35476e41ef2790bcf4813fae0769d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/15/2022
ms.locfileid: "66092202"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/security/cases/ediscoveryCases/{ediscoveryCaseId}/noncustodialDataSources/{ediscoveryNoncustodialDataSourceId}/release')
    .version('beta')
    .post();

```