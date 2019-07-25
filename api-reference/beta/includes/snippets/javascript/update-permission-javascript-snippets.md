---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 92af74ff7f8105926f631ef71f826c8fe3e4321b
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35730524"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const permission = {
  roles: [ "read" ]
};

let res = await client.api('/me/drive/items/{item-id}/permissions/{perm-id}')
    .version('beta')
    .update({permission : permission});

```