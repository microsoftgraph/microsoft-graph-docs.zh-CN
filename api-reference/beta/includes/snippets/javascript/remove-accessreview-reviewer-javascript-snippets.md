---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b8bdb8fdc91b8242eff7d077725996ad7848f87c
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50790465"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/accessReviews/2b83cc42-09db-46f6-8c6e-16fec466a82d/reviewers/006111db-0810-4494-a6df-904d368bd81b')
    .version('beta')
    .delete();

```