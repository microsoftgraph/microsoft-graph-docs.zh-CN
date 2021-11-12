---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9200ae5e3bfaf454580a35b1ea35d887262b915b
ms.sourcegitcommit: 8ae180a32dbd5a2b12512aee64699a2c23b8678b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/14/2021
ms.locfileid: "60561960"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let educationAssignmentResource = await client.api('/education/classes/72a7baec-c3e9-4213-a850-f62de0adad5f/assignments/1618dfb0-3ff2-4edf-8d5c-b8f81df00e80/resources/a7a2fec0-2a26-47bf-8d40-2319c0afb1f4')
    .version('beta')
    .get();

```