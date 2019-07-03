---
description: 自动生成的文件。 不修改
ms.openlocfilehash: c57e7d4a27e35fcad471fa98528b2ef044efa4cb
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35508907"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/directoryRoles')
    .get();

```