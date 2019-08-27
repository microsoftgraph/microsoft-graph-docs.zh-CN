---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 6c8e2ae23f93ec56f3e065ecc7b4f0f6cb4ae27f
ms.sourcegitcommit: 0329bbcd5f1b09a2a6c5f935a30c4560b6eed492
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/27/2019
ms.locfileid: "36636598"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const accessReview = {
    displayName:"TestReview new name"
};

let res = await client.api('/accessReviews/006111db-0810-4494-a6df-904d368bd81b')
    .version('beta')
    .update(accessReview);

```