---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 25ea8ba5b63b1f206265d2ddb274995c306fc992
ms.sourcegitcommit: 6bb3c5c043d35476e41ef2790bcf4813fae0769d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/15/2022
ms.locfileid: "66094753"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/security/cases/eDiscoverycases/58399dff-cebe-478f-b1af-d3227f1fd645/searches/60150269-9758-4439-9bc4-453c864d082f')
    .version('beta')
    .delete();

```