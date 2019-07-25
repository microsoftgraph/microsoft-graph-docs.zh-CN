---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 737dac64a7de1722ebff7f135d80a07c8165e2ba
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35725465"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const sectionGroup = {
  displayName: "Section group name"
};

let res = await client.api('/me/onenote/sectionGroups/{id}/sectionGroups')
    .version('beta')
    .post({sectionGroup : sectionGroup});

```