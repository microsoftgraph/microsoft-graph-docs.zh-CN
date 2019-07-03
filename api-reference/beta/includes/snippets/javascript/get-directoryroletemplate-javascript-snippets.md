---
description: 自动生成的文件。 不修改
ms.openlocfilehash: e37f8fbd82bc98a1fb801bd2a32881c79560756c
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35520286"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/directoryRoleTemplates/{id}')
    .version('beta')
    .get();

```