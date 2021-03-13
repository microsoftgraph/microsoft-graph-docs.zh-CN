---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 213677020a4b6c009ed57f33bc411fa90a2ea8b9
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50798812"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let findRooms = await client.api('/me/findRooms(RoomList='Building2Rooms@contoso.onmicrosoft.com')')
    .version('beta')
    .get();

```