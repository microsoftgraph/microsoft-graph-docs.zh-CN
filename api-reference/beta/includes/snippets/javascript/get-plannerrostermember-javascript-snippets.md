---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 970013e2f7ac582eb9f6f38df4261573b9458393f61c68cc0fe8e6df72db46b0
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57105549"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let plannerRosterMember = await client.api('/planner/rosters/523a9d5a-f9d5-45c1-929f-b8525393515c/members/5ba84f7a-aa11-4a51-a298-9f2c7ec6bb38')
    .version('beta')
    .get();

```