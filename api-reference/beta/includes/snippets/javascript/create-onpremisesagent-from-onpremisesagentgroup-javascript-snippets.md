---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 92242edca0a5013e982c816e49237946698f4908
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35878267"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/onPremisesPublishingProfiles/provisioning/agentGroups')
    .version('beta')
    .post();

```