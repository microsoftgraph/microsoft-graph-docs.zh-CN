---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f3d2ead26387f1f1838a2371e4d99d8d046983a8
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50801332"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const accessReviewReviewer = {
    id: '006111db-0810-4494-a6df-904d368bd81b'
};

await client.api('/accessReviews/2b83cc42-09db-46f6-8c6e-16fec466a82d/reviewers')
    .version('beta')
    .post(accessReviewReviewer);

```