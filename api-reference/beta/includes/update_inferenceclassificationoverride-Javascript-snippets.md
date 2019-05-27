---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 22c427b03471710aa7285942df1742d55f8015b5
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34455840"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const inferenceClassificationOverride = {
  classifyAs: "focused"
};

let res = await client.api('/me/inferenceClassification/overrides/{id}')
    .version('beta')
    .update({inferenceClassificationOverride : inferenceClassificationOverride});

```