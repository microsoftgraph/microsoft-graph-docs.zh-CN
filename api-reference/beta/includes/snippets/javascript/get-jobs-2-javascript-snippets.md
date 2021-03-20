---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5b4176159ac9305c2fb6ac37171e9c11d38ba106
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50950665"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let jobs = await client.api('/print/shares/{id}/jobs')
    .version('beta')
    .get();

```