---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7fc1f1d2cadfd3e8c46034b84558d8aa58cacfe0
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50791892"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/teams/{teamId}/schedule/schedulingGroups/{schedulingGroupId}')
    .version('beta')
    .delete();

```