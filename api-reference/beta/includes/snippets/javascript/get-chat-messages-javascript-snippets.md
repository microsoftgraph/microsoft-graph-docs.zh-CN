---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 29e3d31f41e254305010aa4a211e3335bc62f7e0
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35520967"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/chats/{id}/messages')
    .version('beta')
    .get();

```