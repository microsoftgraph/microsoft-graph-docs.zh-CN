---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d58dffac4f7a336c401ab428d83615bc55f59618
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50951200"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let user = await client.api('/education/me/user')
    .version('beta')
    .get();

```