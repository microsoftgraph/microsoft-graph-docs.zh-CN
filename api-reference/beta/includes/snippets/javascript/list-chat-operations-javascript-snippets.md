---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a2554098e248c12d53aaea93d5e4647c8447eb6d
ms.sourcegitcommit: 7f674112f5b95446fac86d829509f889c60f1693
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/30/2021
ms.locfileid: "53207951"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let operations = await client.api('/chats/19:c253a29b5f694b55a6baad8e83510af7@thread.v2/operations')
    .version('beta')
    .get();

```