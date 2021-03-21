---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4cd1e982bec176ad05c2bbf10462f78cbd65a7a9
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50963198"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const hybridAgentUpdaterConfiguration = {
   updateWindow: 
{
      updateWindowStartTime: '0:00:00',
      updateWindowEndTime: '23:59:00'
  }
};

await client.api('/onPremisesPublishingProfiles/provisioning/hybridAgentUpdaterConfiguration')
    .version('beta')
    .update(hybridAgentUpdaterConfiguration);

```