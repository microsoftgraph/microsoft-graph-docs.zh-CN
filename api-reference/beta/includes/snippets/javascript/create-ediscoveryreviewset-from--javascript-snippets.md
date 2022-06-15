---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3e840da09d1b08a34a1ac7ba558d24da2b0b79fd
ms.sourcegitcommit: 6bb3c5c043d35476e41ef2790bcf4813fae0769d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/15/2022
ms.locfileid: "66095200"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const ediscoveryReviewSet = {
    displayName: 'My review set 2'
};

await client.api('/security/cases/eDiscoverycases/b0073e4e-4184-41c6-9eb7-8c8cc3e2288b/reviewSets')
    .version('beta')
    .post(ediscoveryReviewSet);

```