---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3a4ae05366ab3f74b4853901c6d80d07c509d8f4
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50801295"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/education/synchronizationProfiles/{id}/reset')
    .version('beta')
    .post();

```