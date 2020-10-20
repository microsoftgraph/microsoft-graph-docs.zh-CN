---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0395c9c8cc971bfab2ec2093340ff3ddfa2610fc
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/20/2020
ms.locfileid: "48614097"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/education/classes/11021/assignments/19002/submissions/850f51b7/return')
    .version('beta')
    .post();

```