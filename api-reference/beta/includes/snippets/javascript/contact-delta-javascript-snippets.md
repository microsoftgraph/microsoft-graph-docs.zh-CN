---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 5545f1409e32a7fc718460ca14f590b839d097a9
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35707548"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/contactFolders/{id}/contacts/delta')
    .version('beta')
    .select('displayName')
    .get();

```