---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d4d7f2ca622426410bbb05387225fb4abbb1d1c0
ms.sourcegitcommit: 75428fc7535662f34e965c6b69fef3a53fdaf1cb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/16/2020
ms.locfileid: "49689156"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const presence = {
    ids: ["fa8bf3dc-eca7-46b7-bad1-db199b62afc3", "66825e03-7ef5-42da-9069-724602c31f6b"]
};

let res = await client.api('/communications/getPresencesByUserId')
    .post(presence);

```