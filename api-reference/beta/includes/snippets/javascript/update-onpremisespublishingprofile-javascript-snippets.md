---
description: 自动生成的文件。 不修改
ms.openlocfilehash: a2dfa239ce30f4ed1c4fe1e966d520d9381c9122
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35878251"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const hybridAgentUpdaterConfiguration = {
    "allowUpdateConfigurationOverride" : false
};

let res = await client.api('/onPremisesPublishingProfiles/provisioning/hybridAgentUpdaterConfiguration')
    .version('beta')
    .update({hybridAgentUpdaterConfiguration : hybridAgentUpdaterConfiguration});

```