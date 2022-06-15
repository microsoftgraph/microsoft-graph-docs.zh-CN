---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 13bafa42e4cada34885958264ef7a8fdaf259ec5
ms.sourcegitcommit: 6bb3c5c043d35476e41ef2790bcf4813fae0769d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/15/2022
ms.locfileid: "66094331"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let ediscoveryReviewTag = await client.api('/security/cases/eDiscoverycases/58399dff-cebe-478f-b1af-d3227f1fd645/tags/062de822f17a4a2e9b833aa3f6c37108')
    .version('beta')
    .get();

```