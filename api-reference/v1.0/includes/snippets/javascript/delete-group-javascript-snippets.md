---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 7c1b6c3997b4e2ac4f39d58f11f958fd99369632
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35723378"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/groups/{id}')
    .delete();

```