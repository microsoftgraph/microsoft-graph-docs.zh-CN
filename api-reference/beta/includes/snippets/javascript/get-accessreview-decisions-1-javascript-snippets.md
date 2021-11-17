---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2752afda397f78c3410a1ba79db1f3f2f0eb2259b981a0ea3ea66e5c123c1a69
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56902724"
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