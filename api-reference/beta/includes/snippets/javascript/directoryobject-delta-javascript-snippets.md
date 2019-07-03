---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 3d4848be6ea03b83272c08d28a38b294b45c1078
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35521504"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/directoryObjects/delta')
    .version('beta')
    .filter('isOf('Microsoft.Graph.User')+or+isOf('Microsoft.Graph.Group')')
    .get();

```