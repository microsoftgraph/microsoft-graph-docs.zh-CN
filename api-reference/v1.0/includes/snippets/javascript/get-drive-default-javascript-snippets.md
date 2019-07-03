---
description: 自动生成的文件。 不修改
ms.openlocfilehash: acf2af8d025c2f2ada9b6e1ecdff3a3e82e819d9
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35492999"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/drive')
    .get();

```