---
description: 自动生成的文件。 不修改
ms.openlocfilehash: c0fc90c8b348751ad4eb449ef2240fb71249950e
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35878551"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/onPremisesPublishingProfiles/provisioning/agentGroups/2d55ed41-1619-4848-92bb-0576d3038682/')
    .version('beta')
    .expand('agents')
    .get();

```