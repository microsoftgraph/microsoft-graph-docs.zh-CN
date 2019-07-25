---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 6b24b5a391f601c9f73042f608b9ef7992b7d367
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35726452"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/reports/getYammerActivityCounts(period='D7')')
    .version('beta')
    .get();

```