---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c6f6a3938ed641f86aa79b0301a1e06ff0af2d95
ms.sourcegitcommit: a9731e19589dcb5c0c6fe2e24b008c86573ef803
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/13/2021
ms.locfileid: "49846029"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/directoryObjects/delta')
    .version('beta')
    .filter('isOf('Microsoft.Graph.User') or isOf('Microsoft.Graph.Group')')
    .get();

```