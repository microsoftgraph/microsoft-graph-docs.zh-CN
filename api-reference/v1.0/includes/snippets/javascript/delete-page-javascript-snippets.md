---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 7b3c24aa119cec9f63e8cb2c4b902d0e4ec5822a
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35468121"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/onenote/pages/{id}')
    .delete();

```