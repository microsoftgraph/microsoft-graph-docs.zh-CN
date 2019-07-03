---
description: 自动生成的文件。 不修改
ms.openlocfilehash: ff08acb71ae40c11d2ae987b4dfa5aaa32f9417c
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35520214"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/drive/root/delta?token=latest')
    .version('beta')
    .get();

```