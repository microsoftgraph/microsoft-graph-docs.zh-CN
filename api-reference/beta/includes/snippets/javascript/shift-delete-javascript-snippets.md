---
description: 自动生成的文件。 不修改
ms.openlocfilehash: cbcb478b405302b2e1c70263c5fbfb9a66b83f08
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35480170"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/teams/{teamId}/schedule/shifts/{shiftId}')
    .version('beta')
    .delete();

```