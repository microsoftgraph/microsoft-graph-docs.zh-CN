---
description: 自动生成的文件。 不修改
ms.openlocfilehash: e83d326662cd5aa86ea0f65d86d9524d0cfde494
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35739394"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/reports/getOffice365GroupsActivityDetail(period='D7')')
    .get();

```