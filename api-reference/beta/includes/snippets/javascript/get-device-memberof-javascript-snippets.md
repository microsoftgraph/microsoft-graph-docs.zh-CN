---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 693dedeb0d47b7e2ae20015479e918150ae56902
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35862751"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/devices/{id}/memberOf')
    .version('beta')
    .get();

```