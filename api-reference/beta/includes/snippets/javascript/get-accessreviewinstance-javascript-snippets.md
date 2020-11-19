---
description: 自动生成的文件。请勿修改
ms.openlocfilehash: ec485ce8688eec09d2d552f2c6be9d652c378c44
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49222111"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/identityGovernance/accessReviews/definitions/60860cdd-fb4d-4054-91ba-444404f3baa6/instances/12490cdb-6a18-4c08-ba2c-44442f0a0138')
    .version('beta')
    .get();

```