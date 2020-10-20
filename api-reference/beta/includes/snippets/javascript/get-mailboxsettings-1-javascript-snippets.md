---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c1c50c164319b4b9a1e39f7dfeef2696fff2555d
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/20/2020
ms.locfileid: "48609387"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/mailboxSettings')
    .version('beta')
    .get();

```