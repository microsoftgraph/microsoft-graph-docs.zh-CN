---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 18607d78792acecab821ebdc743cbc76fffa5eaab113fc421a4c02dddc67d096
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57409697"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let plannerProgressTaskBoardTaskFormat = await client.api('/planner/tasks/{task-id}/progressTaskBoardFormat')
    .get();

```