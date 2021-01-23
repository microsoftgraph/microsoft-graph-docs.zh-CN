---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1cafa09af16d6673299e9ff39f17e2a88c96e50f
ms.sourcegitcommit: 9a5facff47a8d4e05ecd2c6cd68294a948c47c4d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2021
ms.locfileid: "49946352"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/print/shares/{id}/jobs')
    .version('beta')
    .get();

```