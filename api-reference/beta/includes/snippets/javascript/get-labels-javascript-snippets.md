---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4f1594d173d983b5a7b10d73f966dfaa5ef56ff1
ms.sourcegitcommit: 9faca60f0cc4ee9d6dce33fd25c72e14b5487d34
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/29/2020
ms.locfileid: "46512271"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/informationProtection/policy/labels')
    .version('beta')
    .get();

```