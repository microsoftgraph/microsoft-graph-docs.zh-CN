---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 22c427b03471710aa7285942df1742d55f8015b5
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35500520"
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