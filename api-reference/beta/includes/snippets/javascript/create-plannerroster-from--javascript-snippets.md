---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: dce50419d23dada38bf555b6c286b2b6d9413bd02ff2ddfd0d34c1a7ccd62b8a
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57158498"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const plannerRoster = {
  '@odata.type': '#microsoft.graph.plannerRoster'
};

await client.api('/planner/rosters')
    .version('beta')
    .post(plannerRoster);

```