---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 74d34e67cc59a7a2c1fcae98dc01136f37bbadee
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50960184"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let namedLocations = await client.api('/identity/conditionalAccess/namedLocations')
    .filter('isof(\'microsoft.graph.ipNamedLocation\')')
    .get();

```