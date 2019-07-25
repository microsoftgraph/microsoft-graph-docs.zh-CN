---
description: 自动生成的文件。 不修改
ms.openlocfilehash: d6f0a5730e14a2620afdbc6f51630a89119da8d7
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35732394"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/messages')
    .select('sender,subject')
    .get();

```