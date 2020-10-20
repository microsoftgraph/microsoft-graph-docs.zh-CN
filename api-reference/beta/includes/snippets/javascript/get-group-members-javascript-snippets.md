---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 624517e7f1bff2c07e29277e2ad8e3c734f5c6ed
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/20/2020
ms.locfileid: "48610357"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/groups/{id}/members')
    .version('beta')
    .get();

```