---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 4c6abeaca3fee0928d1ddec991f79b2c41625cf2
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35875152"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/onPremisesPublishingProfiles/provisioning/publishedResources/aed0b780-965f-4149-85c5-a8c73e58b67d/')
    .version('beta')
    .expand('agentGroups')
    .get();

```