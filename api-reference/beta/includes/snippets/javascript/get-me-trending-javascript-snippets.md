---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3d82816e02818aeb9acdac95cd1524fc9352ecbb
ms.sourcegitcommit: 9faca60f0cc4ee9d6dce33fd25c72e14b5487d34
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/29/2020
ms.locfileid: "46509674"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/insights/trending')
    .version('beta')
    .get();

```