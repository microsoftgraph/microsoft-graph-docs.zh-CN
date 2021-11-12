---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d16ce590c891c2d017b1b9c1a23c0cf2d75273d4
ms.sourcegitcommit: 8ae180a32dbd5a2b12512aee64699a2c23b8678b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/14/2021
ms.locfileid: "60560211"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let educationSubmissionResource = await client.api('/education/classes/72a7baec-c3e9-4213-a850-f62de0adad5f/assignments/1618dfb0-3ff2-4edf-8d5c-b8f81df00e80/submissions/da443246-384d-673b-32db-bdba9d7f2b51/resources/c36626ba-9864-4f3a-8d6f-7104f62df605')
    .get();

```