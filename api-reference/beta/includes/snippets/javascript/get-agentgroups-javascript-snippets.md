---
description: 自动生成的文件。 不修改
ms.openlocfilehash: b05c962c084b261821e1ee93776d5d137bcaa0f4
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35878420"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/onPremisesPublishingProfiles/provisioning/agentGroups')
    .version('beta')
    .expand('publishedResources')
    .get();

```