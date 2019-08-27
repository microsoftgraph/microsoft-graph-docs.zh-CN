---
description: 自动生成的文件。 不修改
ms.openlocfilehash: c9887b517342079486b7b753cb4439a7b60f7d74
ms.sourcegitcommit: 0329bbcd5f1b09a2a6c5f935a30c4560b6eed492
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/27/2019
ms.locfileid: "36636481"
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
    .update(inferenceClassificationOverride);

```