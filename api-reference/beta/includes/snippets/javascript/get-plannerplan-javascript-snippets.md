---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c9cd60866971bda87c42fd62ea28030f724585ff7be7199191bb424f9ae2c32f
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57161392"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let plannerPlan = await client.api('/planner/plans/{id}')
    .version('beta')
    .get();

```