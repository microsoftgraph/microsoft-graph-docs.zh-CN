---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ab8892155990c50a4775281130e60934512e8ed1
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/20/2020
ms.locfileid: "48609878"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/groups/{id}/transitiveMemberOf')
    .get();

```