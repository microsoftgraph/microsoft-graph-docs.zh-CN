---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c42adf7624b652005db3647b20b44319b1b31038
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/20/2020
ms.locfileid: "48620108"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/chats/{id}/messages/{id}/hostedContents')
    .version('beta')
    .get();

```