---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2745ebac9c64f2280a0ee6e6b1b6d414ea06b663
ms.sourcegitcommit: 6bb3c5c043d35476e41ef2790bcf4813fae0769d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/15/2022
ms.locfileid: "66093694"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const ediscoveryReviewTag = {
    displayName: 'My tag API 2',
    description: 'Use Graph API to create tags (updated)'
};

await client.api('/security/cases/eDiscoverycases/58399dff-cebe-478f-b1af-d3227f1fd645/tags/062de822f17a4a2e9b833aa3f6c37108')
    .version('beta')
    .update(ediscoveryReviewTag);

```