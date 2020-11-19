---
description: 自动生成的文件。请勿修改
ms.openlocfilehash: 28334c53ec4583ad6cf4574605de796277b6d246
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49214213"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/identityGovernance/accessReviews/definitions')
    .version('beta')
    .skip(0)
    .top(100)
    .get();

```