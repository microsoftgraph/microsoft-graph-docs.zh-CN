---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 1e80a2e3ff0c3d827d39020ab6aecd04bfa1f38c
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35713011"
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