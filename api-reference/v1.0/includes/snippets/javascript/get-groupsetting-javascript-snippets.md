---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 45c7feee81769947490d4b411bd5e7b226113ce0
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35722458"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/groupSettings/{id}')
    .get();

```