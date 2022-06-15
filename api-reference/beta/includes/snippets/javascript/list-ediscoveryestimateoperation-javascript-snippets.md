---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c8b0c16b34d32fb3b209d4181ab53207f54e4579
ms.sourcegitcommit: 6bb3c5c043d35476e41ef2790bcf4813fae0769d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/15/2022
ms.locfileid: "66092581"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let ediscoveryEstimateOperation = await client.api('/security/cases/eDiscoverycases/b0073e4e-4184-41c6-9eb7-8c8cc3e2288b/searches/c61a5860-d634-4d14-aea7-d82b6f4eb7af/lastEstimateStatisticsOperation')
    .version('beta')
    .get();

```