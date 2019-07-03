---
description: 自动生成的文件。 不修改
ms.openlocfilehash: ecd8776d521e84c950e9562b12ef3e8c412483c2
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35478960"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/findRoomLists')
    .version('beta')
    .get();

```