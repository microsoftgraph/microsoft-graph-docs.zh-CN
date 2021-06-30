---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b356fa59c693f00ae4dd0b38651b0008509d7b9d
ms.sourcegitcommit: 7f674112f5b95446fac86d829509f889c60f1693
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/30/2021
ms.locfileid: "53210659"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const userInsightsSettings = {
  isEnabled: 'false'
};

await client.api('/users/{userId}/settings/itemInsights')
    .version('beta')
    .update(userInsightsSettings);

```