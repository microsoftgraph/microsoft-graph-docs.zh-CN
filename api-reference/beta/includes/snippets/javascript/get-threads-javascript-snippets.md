---
description: 自动生成的文件。 不修改
ms.openlocfilehash: da3279b9ccec73920ac43cc4288ee0d310cda505
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35707241"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/groups/{id}/conversations/{id}/threads')
    .version('beta')
    .get();

```