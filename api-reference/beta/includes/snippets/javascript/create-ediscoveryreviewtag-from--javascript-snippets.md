---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a483398b9ade138872422beb96dfcd76b5333d2d
ms.sourcegitcommit: 6bb3c5c043d35476e41ef2790bcf4813fae0769d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/15/2022
ms.locfileid: "66092135"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let tags = await client.api('/security/cases/eDiscoverycases/58399dff-cebe-478f-b1af-d3227f1fd645/tags')
    .version('beta')
    .get();

```