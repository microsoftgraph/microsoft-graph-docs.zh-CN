---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 0f559bdc28bd55166cfe984f65ed867547a0dd59
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35732415"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const String = {
  securityEnabledOnly: false
};

let res = await client.api('/groups/{id}/getMemberObjects')
    .post(String);

```