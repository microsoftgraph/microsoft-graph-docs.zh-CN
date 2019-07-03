---
description: 自动生成的文件。 不修改
ms.openlocfilehash: b6682a34f9226e32e9eac1953ddf339ade8737b4
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35478638"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/messages')
    .version('beta')
    .select('sender,subject')
    .get();

```