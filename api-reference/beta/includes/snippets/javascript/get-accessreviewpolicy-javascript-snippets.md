---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e60a5fbbd5b23ec1baea7e5c4943be6e90b44f0014069d402d22e0cc6decf9c1
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56902644"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let accessReviewPolicy = await client.api('/policies/accessReviewPolicy')
    .version('beta')
    .get();

```