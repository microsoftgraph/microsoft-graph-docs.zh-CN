---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ce6c203fa066b480c5319ad077f53a2d5d9b6f30
ms.sourcegitcommit: 9edfcf99706c8490cd5832a1c706a88a89e24db1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/07/2020
ms.locfileid: "40871769"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/informationProtection/threatAssessmentRequests')
    .version('beta')
    .get();

```