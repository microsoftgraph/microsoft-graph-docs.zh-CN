---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 93449caadbdbec00b4982d450771b3a2eb3db193
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35712911"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/drive/items/{item-id}/follow')
    .version('beta')
    .post();

```