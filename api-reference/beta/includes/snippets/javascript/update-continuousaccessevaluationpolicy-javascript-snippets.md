---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 18cf890fb379a8e551e0ac36a616fcb326b5ca71
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50783890"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const continuousAccessEvaluationPolicy = {
  '@odata.type': '#microsoft.graph.continuousAccessEvaluationPolicy',
  users: [ '88139f01-1f8d-4c06-ad74-a2544cee9aee' ],
  groups: [ '9972fb3f-7a40-49f5-85f6-129d9dfbd47a', 'ea178055-4713-4d9a-a06c-ff17466b7e77']
};

await client.api('/identity/continuousAccessEvaluationPolicy')
    .version('beta')
    .update(continuousAccessEvaluationPolicy);

```