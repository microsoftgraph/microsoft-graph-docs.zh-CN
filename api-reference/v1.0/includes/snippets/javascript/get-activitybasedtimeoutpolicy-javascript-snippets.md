---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a94b253cfbfb263cfe3cf539e920a79980a3ab8c
ms.sourcegitcommit: 5575e6607817ba23ceb0b01e2f5fc81e58bdcd1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/22/2020
ms.locfileid: "43806270"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/policies/activityBasedTimeoutPolicies/{id}')
    .get();

```