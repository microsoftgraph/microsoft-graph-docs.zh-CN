---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 17d8d75a1437f5dc31bb8c0a78f1107c5d719084ed461323310bcf18909b39f0
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57328931"
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