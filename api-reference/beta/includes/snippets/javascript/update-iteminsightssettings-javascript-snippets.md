---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 789abeb2ffc588d5fd9fc2419b49851e8432aa67
ms.sourcegitcommit: 496410c1e256aa093eabf27f17e820d9ee91a293
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2020
ms.locfileid: "46567062"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const itemInsightsSettings = {
  disabledForGroup: "edbfe4fb-ec70-4300-928f-dbb2ae86c981"
};

let res = await client.api('/organization/{organizationId}/settings/itemInsights')
    .version('beta')
    .update(itemInsightsSettings);

```