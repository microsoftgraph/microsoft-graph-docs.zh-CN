---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 984fcb9e04e35c890f3ae7b5745bd04d5d2d6ad3b5cc465c926d4714eda672c4
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57104306"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let plannerPlan = await client.api('/planner/plans/{plan-id}')
    .get();

```