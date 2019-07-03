---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 7a76b0e690e52c9d7fa86369efef728fa3191af4
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35520292"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/directoryObjects/{id}')
    .version('beta')
    .get();

```