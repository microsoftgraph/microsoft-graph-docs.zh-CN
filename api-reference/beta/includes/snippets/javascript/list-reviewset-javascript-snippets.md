---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 71852a3f11ec4721d09f5fda9ed57f2d0fd9d165
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50776625"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let reviewSets = await client.api('/compliance/ediscovery/cases/{caseId}/reviewSets')
    .version('beta')
    .get();

```