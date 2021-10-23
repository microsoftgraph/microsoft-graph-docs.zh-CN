---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b585af8a9e843774513bf64ac76470cb3ec75b0454c9b93706ca4ea0e2090c50
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57219456"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let continuousAccessEvaluationPolicy = await client.api('/identity/continuousAccessEvaluationPolicy')
    .version('beta')
    .get();

```