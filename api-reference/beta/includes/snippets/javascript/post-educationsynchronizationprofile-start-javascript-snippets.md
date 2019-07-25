---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 1eceaeeb8212ee05cbb8c73b046820cf37cc8f38
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35712444"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/education/synchronizationProfiles/{id}/start')
    .version('beta')
    .post();

```