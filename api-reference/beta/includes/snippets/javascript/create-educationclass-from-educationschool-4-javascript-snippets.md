---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e313d0588d40d8b6dc7f1b173e6a561aed3df9f6
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50951379"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/education/schools/10001/users/13006')
    .version('beta')
    .delete();

```