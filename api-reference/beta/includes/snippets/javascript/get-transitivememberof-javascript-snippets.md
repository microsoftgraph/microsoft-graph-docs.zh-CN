---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 00db367cccc06f7d9e8670176f88bbc5ddf05261
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35716453"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/transitiveMemberOf')
    .version('beta')
    .get();

```