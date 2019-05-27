---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 1e80a2e3ff0c3d827d39020ab6aecd04bfa1f38c
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34446223"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/domains/contoso.com/serviceConfigurationRecords')
    .version('beta')
    .get();

```