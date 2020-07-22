---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ca908d1f082239ab478cb7021eb91727fe6e33bf
ms.sourcegitcommit: 0545b031585e605dc3a0fde481015f51f79819c4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/22/2020
ms.locfileid: "45224830"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/devices/{id}/registeredOwners/{id}/$ref')
    .version('beta')
    .delete();

```