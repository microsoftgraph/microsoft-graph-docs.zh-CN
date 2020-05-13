---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5eb96a7342d0472e212af61cedea8e0e06166337
ms.sourcegitcommit: d4114bac58628527611e83e436132c6581a19c52
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/13/2020
ms.locfileid: "35724424"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/teams/{teamId}/schedule/timeOffReasons/{timeOffReasonId}')
    .version('beta')
    .delete();

```