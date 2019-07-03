---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 9a86f01aa4c583263686edc7d42df94f371e0c1f
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35519840"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/privilegedAccess/azureResources/roleSettings/80dc5d6f-8d89-47b3-953f-01dc909ed3f9')
    .version('beta')
    .get();

```