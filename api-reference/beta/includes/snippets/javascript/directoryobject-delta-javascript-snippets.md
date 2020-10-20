---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3d4848be6ea03b83272c08d28a38b294b45c1078
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/20/2020
ms.locfileid: "48606215"
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