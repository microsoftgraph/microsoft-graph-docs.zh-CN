---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c42e321c55bb4bc947060392fd5a870470e4a5a61ad4d181ab5a544df158d16a
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56902245"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let plannerAssignedToTaskBoardTaskFormat = await client.api('/planner/tasks/{task-id}/assignedToTaskBoardFormat')
    .get();

```