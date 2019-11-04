---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9cf225737d996c1af20bc90090357bebd3ddaeb3
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/02/2019
ms.locfileid: "37938613"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/identity/userFlows/B2C_1_Pol1')
    .version('beta')
    .get();

```