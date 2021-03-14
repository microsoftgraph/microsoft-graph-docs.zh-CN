---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9ec9caeb7e0b3ed3dbbf9b2c3fb9e17fcdaa7fa1
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50789366"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let directReports = await client.api('/contacts/{id}/directReports')
    .get();

```