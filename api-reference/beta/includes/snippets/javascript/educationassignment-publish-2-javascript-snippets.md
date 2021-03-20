---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 557887a6869990c43c7376819f023f18fdc72c29
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50951759"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/education/classes/11021/assignments/19002/publish')
    .version('beta')
    .post();

```