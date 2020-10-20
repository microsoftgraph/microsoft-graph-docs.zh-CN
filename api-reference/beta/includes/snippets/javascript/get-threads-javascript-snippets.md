---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: da3279b9ccec73920ac43cc4288ee0d310cda505
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/20/2020
ms.locfileid: "48605863"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/groups/{id}/conversations/{id}/threads')
    .version('beta')
    .get();

```