---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3a48e9b685c977619a5a69b7d40b8da9ad78f984
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50773156"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/compliance/ediscovery/cases/{caseId}/legalHolds/{legalholdId}')
    .version('beta')
    .delete();

```