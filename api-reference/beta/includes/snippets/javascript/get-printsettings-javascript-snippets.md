---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 673a43c7b73f4714533b264db142718ff2debbda
ms.sourcegitcommit: 33ffed5b785abf36b1a7786856c9266958830d25
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/25/2020
ms.locfileid: "42948347"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/print/settings')
    .version('beta')
    .get();

```