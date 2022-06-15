---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0341a1a684d11562be39b0eafcc6c5eaeb98b1f3
ms.sourcegitcommit: 6bb3c5c043d35476e41ef2790bcf4813fae0769d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/15/2022
ms.locfileid: "66093881"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let run = await client.api('/security/cases/eDiscoverycases/58399dff-cebe-478f-b1af-d3227f1fd645/reviewSets/273f11a1-17aa-419c-981d-ff10d33e420f/queries/837335b0-1943-444d-a3d1-5522cc21c5a4/run')
    .version('beta')
    .get();

```