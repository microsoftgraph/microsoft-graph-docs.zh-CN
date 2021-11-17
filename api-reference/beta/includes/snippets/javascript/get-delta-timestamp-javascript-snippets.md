---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8b9d0696ded542930d4c053f10effa62b57d5177
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61019923"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let delta = await client.api('/me/drive/root/delta?token=2021-09-29T20%3A00%3A00Z')
    .version('beta')
    .get();

```