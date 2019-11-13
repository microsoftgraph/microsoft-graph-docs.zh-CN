---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d6c8e5da6af93fc1e31d8c22d39135fbf039ec11
ms.sourcegitcommit: fa08172601324fc01b090f8135fba4600bd1a9f8
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/13/2019
ms.locfileid: "38302775"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/communications/calls/{id}/audioRoutingGroups/{id}')
    .version('beta')
    .delete();

```