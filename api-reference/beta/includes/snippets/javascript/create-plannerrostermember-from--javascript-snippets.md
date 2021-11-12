---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 542eee0cf75632769b7f287596fc20c332ac8eb4dc225046501763b43c66ad92
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57273961"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const plannerRosterMember = {
  '@odata.type': '#microsoft.graph.plannerRosterMember',
  userId: 'String'
};

await client.api('/planner/rosters/6519868f-868f-6519-8f86-19658f861965/members')
    .version('beta')
    .post(plannerRosterMember);

```