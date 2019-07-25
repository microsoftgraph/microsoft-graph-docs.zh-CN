---
description: 自动生成的文件。 不修改
ms.openlocfilehash: cffc768a17ba60e652efa224acf4963b0b5bc7fa
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35713584"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/groups/{id}/transitiveMembers')
    .version('beta')
    .get();

```