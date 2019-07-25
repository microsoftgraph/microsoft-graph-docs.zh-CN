---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 0728b7c15435ab4417edcc127e8d03a4907117cb
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35730139"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/onenote/notebooks/getRecentNotebooks(includePersonalNotebooks=true)')
    .get();

```