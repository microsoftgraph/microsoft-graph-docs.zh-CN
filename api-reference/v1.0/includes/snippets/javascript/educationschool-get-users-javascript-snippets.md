---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c8d2e609e526da18930bbe626d8b1585012433ed
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50804466"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let users = await client.api('/education/schools/{school-id}/users')
    .get();

```