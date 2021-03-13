---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 274085a0f15a67d35228b8602c18a75b98582ff9
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50800516"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let calendars = await client.api('/me/calendars')
    .version('beta')
    .get();

```