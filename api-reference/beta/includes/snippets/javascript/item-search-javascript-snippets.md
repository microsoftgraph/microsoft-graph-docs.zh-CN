---
description: 自动生成的文件。 不修改
ms.openlocfilehash: d8033f8b6803ebd674b8593428aa86e14e0a5cf2
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35705839"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/drive/root/search(q='{search-query}')')
    .version('beta')
    .get();

```