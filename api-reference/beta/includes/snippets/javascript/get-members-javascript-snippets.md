---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 29992c62d99137b67db52825953372417bade8db
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35705646"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/education/classes/11016/members')
    .version('beta')
    .get();

```