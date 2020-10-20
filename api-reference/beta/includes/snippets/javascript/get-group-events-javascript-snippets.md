---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ede3a5c2d8880becb5f35825177ce31c5bb79fd7
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/20/2020
ms.locfileid: "48608972"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/groups/{id}/events')
    .version('beta')
    .get();

```