---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: cbcb478b405302b2e1c70263c5fbfb9a66b83f08
ms.sourcegitcommit: d4114bac58628527611e83e436132c6581a19c52
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/13/2020
ms.locfileid: "35725246"
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