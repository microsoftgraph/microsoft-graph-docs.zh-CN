---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 7879beb10ea5ab20b9a3ea2daa777b8a644488e0
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35478419"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/onenote/sectionGroups/{id}/sectionGroups')
    .version('beta')
    .get();

```