---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 06a28fc5b4074cefbcbb1a0566dbf0e682b6177a
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50789860"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const itemInsightsSettings = {
  disabledForGroup: 'edbfe4fb-ec70-4300-928f-dbb2ae86c981'
};

await client.api('/organization/{organizationId}/settings/itemInsights')
    .version('beta')
    .update(itemInsightsSettings);

```