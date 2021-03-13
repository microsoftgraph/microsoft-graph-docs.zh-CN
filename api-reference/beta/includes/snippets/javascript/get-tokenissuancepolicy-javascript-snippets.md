---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 638a95b5c9337f44f15d834cb314c88808b2f98b
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50782949"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let tokenIssuancePolicy = await client.api('/policies/tokenIssuancePolicies/{id}')
    .version('beta')
    .get();

```