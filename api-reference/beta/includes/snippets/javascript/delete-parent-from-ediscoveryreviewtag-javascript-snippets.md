---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8484257bb58644d28b29be5c6e321e648db10769
ms.sourcegitcommit: 6bb3c5c043d35476e41ef2790bcf4813fae0769d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/15/2022
ms.locfileid: "66095359"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/security/cases/eDiscoverycases/58399dff-cebe-478f-b1af-d3227f1fd645/tags/d05c2ef9369d49c293b5a6a6d18a5fd9')
    .version('beta')
    .delete();

```