---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: aa9ca613351bec6c582e8fbae10b9f2fda17f86f
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50785548"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const inferenceClassificationOverride = {
  classifyAs: 'focused'
};

await client.api('/me/inferenceClassification/overrides/{id}')
    .version('beta')
    .update(inferenceClassificationOverride);

```