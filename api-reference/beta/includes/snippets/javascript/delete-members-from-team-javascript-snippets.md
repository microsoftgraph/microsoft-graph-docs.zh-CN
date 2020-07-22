---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: cde3250f46fe241c758fc3773ad8d0c27a1d4fac
ms.sourcegitcommit: 0545b031585e605dc3a0fde481015f51f79819c4
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/22/2020
ms.locfileid: "45225838"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/teams/{teamsId}/members/{membership-id}')
    .version('beta')
    .delete();

```