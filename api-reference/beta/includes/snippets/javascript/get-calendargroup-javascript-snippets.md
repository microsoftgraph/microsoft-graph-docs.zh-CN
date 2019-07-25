---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 67744a98619020efb2f65bfe4a791aa33422b130
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35709110"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/calendarGroups/{id}')
    .version('beta')
    .get();

```