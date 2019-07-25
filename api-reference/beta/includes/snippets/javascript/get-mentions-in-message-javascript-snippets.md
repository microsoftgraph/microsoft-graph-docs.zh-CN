---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 38e4f6494806b97cc4a77f20e95e07c4418ad6fc
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35729808"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/messages/AQMkADJmMTUAAAgVZAAAA/')
    .version('beta')
    .expand('mentions')
    .get();

```