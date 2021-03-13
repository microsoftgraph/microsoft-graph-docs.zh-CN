---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9da09328f28f5c153f886806fbbc7c65ce31096c
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50804922"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let messages = await client.api('/me/messages')
    .version('beta')
    .select('sender,subject')
    .get();

```