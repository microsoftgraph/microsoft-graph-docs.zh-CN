---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d0676a47c7c90079b917c0f1f5583fa7e6a2c79b
ms.sourcegitcommit: 54ba08a80db85b9e84813387e8c4416eca44fa8e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/26/2022
ms.locfileid: "65695262"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/chats/19:cf66807577b149cca1b7af0c32eec122@thread.v2/pinnedMessages/1616964509832')
    .version('beta')
    .delete();

```