---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 735cd4b244a1d97dfd3bf3a7a4044c6496c409be
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35722249"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/reports/getYammerGroupsActivityGroupCounts(period='D7')')
    .get();

```