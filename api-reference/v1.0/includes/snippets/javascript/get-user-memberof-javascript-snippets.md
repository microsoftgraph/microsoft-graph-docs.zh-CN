---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 770166e1fe7c3766b01188de60e3623f6a6acc13
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35468131"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/devices/{id}/memberOf')
    .get();

```