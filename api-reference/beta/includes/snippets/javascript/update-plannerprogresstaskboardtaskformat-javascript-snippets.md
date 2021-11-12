---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4da814b04042d29974dc129494660ce09d24a1752702a30e2f3f1648a7ca8365
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57273973"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const plannerProgressTaskBoardTaskFormat = {
  orderHint: 'A6673H Ejkl!'
};

await client.api('/planner/tasks/{id}/progressTaskBoardFormat')
    .version('beta')
    .update(plannerProgressTaskBoardTaskFormat);

```