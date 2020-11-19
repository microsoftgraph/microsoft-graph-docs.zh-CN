---
description: 自动生成的文件。请勿修改
ms.openlocfilehash: 2ec862b55f579e7daa41813b66a6a2453abae3ce
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49214738"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/identityGovernance/accessReviews/definitions/60860cdd-fb4d-4054-91ba-f75e04f34444/instances')
    .version('beta')
    .skip(0)
    .top(100)
    .get();

```