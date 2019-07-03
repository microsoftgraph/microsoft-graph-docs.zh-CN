---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 0728b7c15435ab4417edcc127e8d03a4907117cb
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35510048"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/onenote/notebooks/getRecentNotebooks(includePersonalNotebooks=true)')
    .get();

```