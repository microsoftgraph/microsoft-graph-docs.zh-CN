---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2fed6776d3890cfa0542568e7ecfcffd42a851bc
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50806080"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let relations = await client.api('/termStore/sets/{setId}/relations')
    .version('beta')
    .get();

```