---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: db911671d1b74faf586141c5743c0cb909099609
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/20/2020
ms.locfileid: "48617777"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/contacts/{id}')
    .version('beta')
    .delete();

```