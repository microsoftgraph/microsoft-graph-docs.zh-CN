---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 0395c9c8cc971bfab2ec2093340ff3ddfa2610fc
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35500576"
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