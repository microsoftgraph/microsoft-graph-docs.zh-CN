---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 22ee822aa2307dcc1d3b11565ab4a0d21b2d971f
ms.sourcegitcommit: fe1b4d098af604cc34596f595e799911ea672532
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/07/2021
ms.locfileid: "51611652"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let chatMessage = await client.api('/teams/fbe2bf47-16c8-47cf-b4a5-4b9b187c508b/channels/19:4a95f7d8db4c4e7fae857bcebe0623e6@thread.tacv2/messages/1612509044972/replies/1613671348387')
    .get();

```