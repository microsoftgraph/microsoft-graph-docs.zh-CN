---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 876059e3219481f8a77a57f21fca61bccaf198a4
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50781793"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let chatMessage = await client.api('/teams/{id}/channels/{id}/messages/delta')
    .top(2)
    .get();

```