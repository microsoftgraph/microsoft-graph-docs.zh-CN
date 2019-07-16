---
description: 自动生成的文件。 不修改
ms.openlocfilehash: e0a1372f8f0fecfde1126b49b720dc073a805ed5
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35740355"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const calendarGroup = {
  name: "name-value"
};

let res = await client.api('/me/calendarGroups/{id}')
    .update({calendarGroup : calendarGroup});

```