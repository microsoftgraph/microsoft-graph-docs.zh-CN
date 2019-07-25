---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 777ea8bafe5ac5673f9f6eb3a0d3c5060bb3d36e
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35732115"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/mailFolders/{id}/messages/delta')
    .header('Prefer','odata.maxpagesize=2')
    .get();

```