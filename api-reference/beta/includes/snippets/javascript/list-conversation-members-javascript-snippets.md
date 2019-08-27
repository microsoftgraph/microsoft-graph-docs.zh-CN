---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5039c8e7e58a08a3da225119fdfe8135d7617806
ms.sourcegitcommit: 0329bbcd5f1b09a2a6c5f935a30c4560b6eed492
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/27/2019
ms.locfileid: "36633333"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/chats/{id}/members')
    .version('beta')
    .get();

```