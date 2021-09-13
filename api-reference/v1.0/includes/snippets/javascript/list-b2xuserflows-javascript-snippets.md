---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0c787156eb475645728d4cbfb4f23d4cf32ab7aaee02284d5951c0d621840025
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57333932"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let b2xUserFlows = await client.api('/identity/b2xUserFlows')
    .get();

```