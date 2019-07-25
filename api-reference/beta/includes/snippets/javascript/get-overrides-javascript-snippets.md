---
description: 自动生成的文件。 不修改
ms.openlocfilehash: c6a0fc91fa0adbd4aec8036990ca96a1ae3d9670
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35711619"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/inferenceClassification/overrides')
    .version('beta')
    .get();

```