---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4bed8e7eed48ace7e017a01bd440f8925fffdb2e
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50943164"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let decisions = await client.api('/accessReviews/2b83cc42-09db-46f6-8c6e-16fec466a82d/decisions')
    .version('beta')
    .get();

```