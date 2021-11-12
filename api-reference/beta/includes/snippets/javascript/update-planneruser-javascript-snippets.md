---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 45d040407ac0c501416b41024ff5b40398ea4dfd93d54a415422f2f1646ea336
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57164186"
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