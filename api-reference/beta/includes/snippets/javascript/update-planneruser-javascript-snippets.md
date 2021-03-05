---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: cb35eb176d34218547834661ff55a4f9822d4e10
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2021
ms.locfileid: "50474030"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const plannerUser = {
  favoritePlanReferences: {
    jd8S5gOaFk2S8aWCIAJz42QAAxtD: {
      '@odata.type': '#microsoft.graph.plannerFavoritePlanReference',
      orderHint: ' !',
      planTitle: 'Next Release Discussion'
    },
    '7oTB5aMIAE2rVo-1N-L7RmQAGX2q': null
  },
  recentPlanReferences: {
    jd8S5gOaFk2S8aWCIAJz42QAAxtD: {
      '@odata.type': '#microsoft.graph.plannerRecentPlanReference',
      lastAccessedDateTime: '2018-01-02T22:49:46.155Z',
      planTitle: 'Next Release Discussion'
    }
  }
};

await client.api('/me/planner')
    .version('beta')
    .update(plannerUser);

```