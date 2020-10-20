---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 93449caadbdbec00b4982d450771b3a2eb3db193
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/20/2020
ms.locfileid: "48613965"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/drive/items/{item-id}/follow')
    .version('beta')
    .post();

```