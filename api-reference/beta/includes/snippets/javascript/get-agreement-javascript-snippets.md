---
description: 自动生成的文件。 不修改
ms.openlocfilehash: bd0fcd02bf174e1058ae5be8f40f81dcef4a2191
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35478361"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/agreements/'id'')
    .version('beta')
    .expand('files')
    .get();

```