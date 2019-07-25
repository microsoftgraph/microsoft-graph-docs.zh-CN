---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 6ef99c775f32ba97eae10de4479bf072a289baf3
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35864924"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/calendarGroups/{id}/calendars')
    .version('beta')
    .get();

```