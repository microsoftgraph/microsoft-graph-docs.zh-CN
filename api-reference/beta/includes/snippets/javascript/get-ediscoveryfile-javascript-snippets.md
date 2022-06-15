---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f68832bf50c2710565d057068c542f94dcb77d97
ms.sourcegitcommit: 6bb3c5c043d35476e41ef2790bcf4813fae0769d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/15/2022
ms.locfileid: "66093000"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let ediscoveryFile = await client.api('/security/cases/eDiscoverycases/58399dff-cebe-478f-b1af-d3227f1fd645/reviewSets/273f11a1-17aa-419c-981d-ff10d33e420f/files/000168cdf05c48d98faac7bff8719726a25da40bb2b9c369fb580b8797abf661')
    .version('beta')
    .get();

```