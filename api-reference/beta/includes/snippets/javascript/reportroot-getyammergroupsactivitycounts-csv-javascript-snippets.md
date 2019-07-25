---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 7a20035c8ef81b69eedf9be30975213c730cef11
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35726293"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/reports/getYammerGroupsActivityCounts(period='D7')')
    .version('beta')
    .get();

```