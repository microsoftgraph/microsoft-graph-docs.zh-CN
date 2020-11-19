---
description: 自动生成的文件。请勿修改
ms.openlocfilehash: eaee8397614f806438c7bb5bdb82f50ab87dfc58
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49214351"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/identityGovernance/accessReviews/definitions/60860cdd-fb4d-4054-91ba-444404f3baa6/instances/14444cdb-6a18-4c08-ba2c-48c02f0a0138/decisions')
    .version('beta')
    .skip(0)
    .top(100)
    .get();

```