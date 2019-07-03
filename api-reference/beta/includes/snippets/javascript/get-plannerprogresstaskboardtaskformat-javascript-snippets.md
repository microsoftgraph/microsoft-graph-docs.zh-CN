---
description: 自动生成的文件。 不修改
ms.openlocfilehash: a3f678005ebb6cab695e5573b4636bcc2b9a88ed
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35521352"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/planner/tasks/'id'/progressTaskBoardFormat')
    .version('beta')
    .get();

```