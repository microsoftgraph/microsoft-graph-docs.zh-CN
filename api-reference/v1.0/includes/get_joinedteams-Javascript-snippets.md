---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 5e72c61ae60ac6a69bc28309855f8cd914008220
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34457304"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/joinedTeams')
    .get();

```