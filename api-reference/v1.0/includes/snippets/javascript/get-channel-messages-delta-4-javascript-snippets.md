---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a195bf6917b6abc5b1222714c0baf23bc5c70ed4
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50781604"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let chatMessage = await client.api('/teams/{id}/channels/{id}/messages/delta')
    .get();

```