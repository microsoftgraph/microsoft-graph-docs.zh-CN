---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 365bbe4f3540f4b46a96d605d3fbb1bf34853276
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35705463"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const String = {
  securityEnabledOnly: false
};

let res = await client.api('/groups/{id}/getMemberGroups')
    .version('beta')
    .post(String);

```