---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d8ab62c60873ebe4afa93a3061be9e260a1117ba
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65220338"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let signIns = await client.api('/auditLogs/signIns')
    .filter('startsWith(appDisplayName,\'Graph\')')
    .top(10)
    .get();

```