---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 31cb3a18476c1b94d82e234bf7c6c0e517350c85
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/20/2020
ms.locfileid: "48617725"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/messages/AAMkADYAAAImV_jAAA=/')
    .version('beta')
    .expand('eventMessage/event')
    .get();

```