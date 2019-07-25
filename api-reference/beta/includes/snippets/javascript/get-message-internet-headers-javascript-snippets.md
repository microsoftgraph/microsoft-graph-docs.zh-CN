---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 631b66ef72c9618d381e18cb96f761c9d2eaf541
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35729816"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/messages/AAMkAGVmMDEz/')
    .version('beta')
    .select('internetMessageHeaders')
    .get();

```