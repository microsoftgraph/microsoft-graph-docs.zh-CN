---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f243e82eadeabc0931084cbbb74be1f1760ab267
ms.sourcegitcommit: d4114bac58628527611e83e436132c6581a19c52
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/13/2020
ms.locfileid: "44217048"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/teams/{teamId}/schedule/timeOffRequests')
    .version('beta')
    .get();

```