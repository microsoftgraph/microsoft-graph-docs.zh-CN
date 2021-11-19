---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d3a77991a070286553af547968007039885b26fa
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61102763"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let insightsSettings = await client.api('/organization/{organizationId}/settings/itemInsights')
    .version('beta')
    .get();

```