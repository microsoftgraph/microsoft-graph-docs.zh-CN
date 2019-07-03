---
description: 自动生成的文件。 不修改
ms.openlocfilehash: ee7b8bf37e7556c58e407807802ed5bb0e87cc72
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35479496"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/applicationTemplates/{id}')
    .version('beta')
    .get();

```