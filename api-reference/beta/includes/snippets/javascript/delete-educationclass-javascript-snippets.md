---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a53b1c1d0a4c51ecacb696cdc58e6ddd7f73c0c8
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50800274"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/education/classes/11022')
    .version('beta')
    .delete();

```