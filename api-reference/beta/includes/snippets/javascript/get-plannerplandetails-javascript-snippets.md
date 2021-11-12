---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f26e4b105220fd17a4f45b8f959cca8dc82f937f911b55a326566f17518b48c2
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57332879"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let plannerPlanDetails = await client.api('/planner/plans/xqQg5FS2LkCp935s-FIFm2QAFkHM/details')
    .version('beta')
    .get();

```