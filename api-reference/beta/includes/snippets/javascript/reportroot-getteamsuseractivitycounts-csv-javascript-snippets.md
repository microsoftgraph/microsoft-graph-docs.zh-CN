---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 44c752f47a707484314f3cfa8b4a546dd6ffdc34
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35726546"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/reports/getTeamsUserActivityCounts(period='D7')')
    .version('beta')
    .get();

```