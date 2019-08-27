---
description: 自动生成的文件。 不修改
ms.openlocfilehash: ac4b4efef8e3465087b3fcfc8fadacf813c197bf
ms.sourcegitcommit: 0329bbcd5f1b09a2a6c5f935a30c4560b6eed492
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/27/2019
ms.locfileid: "36636480"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const accessReviewReviewer = {
    id:"006111db-0810-4494-a6df-904d368bd81b"
};

let res = await client.api('/accessReviews/2b83cc42-09db-46f6-8c6e-16fec466a82d/reviewers')
    .version('beta')
    .post(accessReviewReviewer);

```