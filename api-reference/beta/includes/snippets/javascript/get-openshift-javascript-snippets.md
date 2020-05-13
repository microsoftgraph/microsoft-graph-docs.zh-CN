---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1e66d56861aa980b94530fd8a8e1e87475437249
ms.sourcegitcommit: d4114bac58628527611e83e436132c6581a19c52
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/13/2020
ms.locfileid: "40867759"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/teams/{id}/schedule/openShifts')
    .version('beta')
    .get();

```