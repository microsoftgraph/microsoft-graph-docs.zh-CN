---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9837358bb5959af9e36c79216af13e71fa61d717
ms.sourcegitcommit: 60ced1be6ed8dd2d23263090a1cfbc16689bb043
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/28/2020
ms.locfileid: "48782993"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/chats/{id}/members')
    .get();

```